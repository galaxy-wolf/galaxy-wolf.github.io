---
layout:  article 
title:  个人主页搭建
categories:  setup
tags: 本地部署

---

#简介

[github page](https://pages.github.com) 是github为个人主页和项目主页提供的免费托管服务。由于其高度的可定制性，是程序员
博客的不二选择。缺点是只能做静态网页。

本主页使用了名为[skinny bones](http://mmistakes.github.io/skinny-bones-jekyll/) 的jekyll模板，在模板得主页上有其详细的使用说明, [jekyll](http://jekyllrb.com) 是一个博客网站生成器，能够方便博客得编写。

搭建过程也比较简单，首先按照[github page](https://pages.github.com/)的说明，在github上建立主页项目,然后是搭建jekyll在本地运行环境，方便本地预览。最后是安装模板, 下面着重讲一下jekyll的安装过程。

##Step 1 创建主页项目

具体内容参考[github page](https://pages.github.com/).

##Step 2 安装 jekyll 

jekyll 是基于ruby的一个软件，因此依赖得软件有：ruby ruby-devel 以及gun的c编译环境等。

####[在OpenSuse下安装过程](http://www.snip2code.com/Snippet/126790/Install-Jekyll-on-OpenSuse-13-1)：

{% highlight powershell%}
zypper in -t pattern devel_basis
zypper in ruby-devel
zypper in nodejs
gem install jekyll
gem install execjs
{% endhighlight %}

**info Notice:** 在使用gem之前，要将ruby源换为淘宝的源，具体方法如下:
{: .notice-info}
{% highlight powershell%}
gem sources --remove https://rubygems.org/
gem sources -a http://ruby.taobao.org/ 
{% endhighlight %}

##Step 3 安裝模板

在模板的说明文档中有详细说明[说明文档](http://mmistakes.github.io/skinny-bones-jekyll/getting-started/).


