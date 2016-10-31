# opensource.ynu.edu.cn
The official static site of opensource-yunnan-university

# 如何搭建环境

1. 安装`git`、`python`等工具
2. 安装`pelican`，执行`pip install pelican markdown ghp-import`
3. 下载本项目，执行`git clone https://github.com/opensource-yunnan-university/opensource.ynu.edu.cn.git`
4. 编译和预览，在项目更目录下执行`make html && make serve`

# 如何添加内容

添加的内容放在`content`目录下面，使用英文文件名，如果有多个单词，则使用`-`连字符，后缀是`md`，在markdown文件的开始部分需要添加`metadata`，然后空一行再写内容，具体格式如下，可参考官方的 [Writing content][Writing content]

```markdown
Title: My super title
Date: 2010-12-03 10:20
Modified: 2010-12-05 19:30
Category: Python
Tags: pelican, publishing
Slug: my-super-post
Authors: Alexis Metaireau, Conan Doyle
Summary: Short version for index and feeds

This is the content of my super blog post.
```

注意这里的Category目前支持的有`Event`、`Blog`、`Podcast`这几种

# 如何编译和预览

在项目根目录下执行`make html && make serve`，然后打开浏览器浏览[http://localhost:8000/](http://localhost:8000/)就可以，一般为了提升修改-预览-修改效率，可以在一个shell session中`make serve`，另一个shell session中每当更新内容之后再次执行`make html`

# 如何提交内容

1.  如果是云大开源中心会员，`clone`本项目之后修改内容，直接`push`
2.  其他用户，请先`fork`之后添加内容，然后`send pull request`给我们，我们审核通过后就会更新。

# 开源协议

本项目使用[Apache License Version 2.0](http://www.apache.org/licenses/)开源协议

# 参考资料
1. [Markdown-Cheatsheet][Markdown-Cheatsheet]
2. [How to set up Pelican on GitHub pages][How to set up Pelican on GitHub pages]
3. [pelican-themes][pelican-themes]
4. [pelican-plugins][pelican-plugins]
5. [Coding An HTML 5 Layout From Scratch][Coding An HTML 5 Layout From Scratch]
6. [www.tuna.moe][www.tuna.moe]

[Writing content]: http://docs.getpelican.com/en/3.6.3/content.html
[Markdown-Cheatsheet]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[How to set up Pelican on GitHub pages]: http://railslide.io/pelican-github-pages.html
[pelican-themes]: https://github.com/getpelican/pelican-themes
[pelican-plugins]: [https://github.com/getpelican/pelican-plugins]
[www.tuna.moe]: [https://www.tuna.moe/]
[Coding An HTML 5 Layout From Scratch]: [https://www.smashingmagazine.com/2009/08/designing-a-html-5-layout-from-scratch/]