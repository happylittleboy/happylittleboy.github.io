---
layout: post
title:  "Leaning jekyll"
date:   2016-11-22 08:45:18 +0800
categories: ruby
---
首先确认本地机器上安装过`Ruby`、`RubyGems`，安装`jekyll`：
{% highlight shell %}
	$ gem install jekyll #安装jekyll
	$ jekyll --version #查看当前jekyll版本
	$ gem list jekyll #也可以查看当前jekyll版本
	$ gem update jekyll #更新
{% endhighlight %}
创建工作目录：
{% highlight shell %}
	$ jekyll new myblog #在当前目录下创建jekyll工作目录myblog，`jekyll new`会自动初始化`bundle install`
	$ jekyll new myblog --skip-bundle #跳过自动初始化`bundle install`
{% endhighlight %}
默认情况下，站点文件会生成到_site目录下，如果更改目录可以`$ bundle exec jekyll build --destination <destination>`：
{% highlight shell %}
	$ bundle exec jekyll build --destination _newsite #生成到当前目录下的`_newsite`目录下
{% endhighlight %}

