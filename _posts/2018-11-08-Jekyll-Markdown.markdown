---
layout: post
title:  把Jekyll和Markdown的常用语法用得66
date:   2018-11-08
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: post-5.jpg # Add image post (optional)
tags: [Jekyll]
author: 姜戈# Add name author (optional)
jekyll: true
---
因为常写博客和网站搭建，经常用到Jekyll和Markdown，备忘下常用语法。
# Markdown常用语法
Markdown 的优点如下：

1. 纯文本，所以兼容性极强，可以用所有文本编辑器打开。
2. 让你专注于文字而不是排版。
3. 格式转换方便，Markdown 的文本你可以轻松转换为 html、电子书等。
4. Markdown 的标记语法有极好的可读性。

## 标题

这是最为常用的格式，在平时常用的的文本编辑器中大多是这样实现的：输入文本、选中文本、设置标题格式。

而在 Markdown 中，你只需要在文本前面加上 `#` 即可，同理、你还可以增加二级标题、三级标题、四级标题、五级标题和六级标题，总共六级，只需要增加 `#` 即可，标题字号相应降低。例如：

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题 

```

*注：`#` 和「一级标题」之间建议保留一个字符的空格，这是最标准的 Markdown 写法。*

*你可以你的编辑器中尝试输入这六级标题，可以参考下方的截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-46c9de182ac8b3c3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 列表

列表格式也很常用，在 Markdown 中，你只需要在文字前面加上 `-` 就可以了，例如：

```
- 文本1
- 文本2
- 文本3

```

如果你希望有序列表，
也可以在文字前面加上 `1.` `2.` `3.` 就可以了，例如：

```
1\. 文本1
2\. 文本2
3\. 文本3

```

*注：`-`、`1.`和文本之间要保留一个字符的空格。*

*列表案例截图如下：*

![](https://upload-images.jianshu.io/upload_images/13813710-cacc7581a600092b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


在 Markdown 中，插入链接不需要其他按钮，你只需要使用 `[显示文本](链接地址)` 这样的语法即可，例如：

```
[简书](http://www.jianshu.com)

```

在 Markdown 中，插入图片不需要其他按钮，你只需要使用这样`[](图片链接地址)` 的语法即可，例如：

```
![](http://upload-images.jianshu.io/upload_images/259-0ad0d0bfc1c608b6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

```

*注：插入图片的语法和链接的语法很像，只是前面多了一个 `！`。*

*插入链接和图片的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-4e9ad2e76bce721c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 引用

在我们写作的时候经常需要引用他人的文字，这个时候引用这个格式就很有必要了，在 Markdown 中，你只需要在你希望引用的文字前面加上 `>` 就好了，例如：

```
> 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

```

*注：`>` 和文本之间要保留一个字符的空格。*

最终显示的就是：

> 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

*引用的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-6d4a813c14bdced6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 粗体和斜体

Markdown 的粗体和斜体也非常简单，用两个 `*` 包含一段文本就是粗体的语法，用一个 `*` 包含一段文本就是斜体的语法。例如：

```
 *一盏灯*， 一片昏黄；**一简书**， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

```

最终显示的就是下文，其中「一盏灯」是斜体，「一简书」是粗体：

*一盏灯*， 一片昏黄；**一简书**， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

*粗体和斜体的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-5596c573dc7787f0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 代码引用

需要引用代码时，如果引用的语句只有一段，不分行，可以用 ` 将语句包起来。
如果引用的语句为多行，可以将```置于这段代码的首行和末行。
*代码引用的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-79c0c6de3c111cb9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 表格

相关代码：

```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```

显示效果：

| Tables | Are | Cool |
| --- | --- | --- |
| col 3 is | right-aligned | $1600 |
| col 2 is | centered | $12 |
| zebra stripes | are neat | $1 |

<p></p>
相关代码：

```
dog | bird | cat
----|------|----
foo | foo  | foo
bar | bar  | bar
baz | baz  | baz

```

显示效果：

| dog | bird | cat |
| --- | --- | --- |
| foo | foo | foo |
| bar | bar | bar |
| baz | baz | baz |

<p></p>

## 显示链接中带括号的图片

![][1]
[1]: [http://latex.codecogs.com/gif.latex](https://link.jianshu.com?t=http://latex.codecogs.com/gif.latex)?\prod%20(n_{i})+1

代码如下:

```
![][1]
[1]: http://latex.codecogs.com/gif.latex?\prod%20\(n_{i}\)+1
```

# Jekyll常用语法
## **Jekyll 目录结构**

jekyll目录结构主要包含如下目录：

> _posts 博客内容
> _pages 其他需要生成的网页，如About页
> _layouts 网页排版模板
> _includes 被模板包含的HTML片段，可在_config.yml中修改位置
> assets 辅助资源 css布局 js脚本 图片等
> _data 动态数据
> _sites 最终生成的静态网页
> _config.yml 网站的一些配置信息
> index.html 网站的入口

那么这些目录是如何运作的呢？

1.  我们打开根目录下的index.html可以看到：

    > —
    > layout: home-page
    > —
    > **html代码段**

2.  上面的home-page我们到_layouts目录下可以找到：

    ![image.png](https://upload-images.jianshu.io/upload_images/13813710-51cadf0bf21bbb6a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


    实际上根目录下index.html运行后是home-page里面的代码内容，1中**html代码段**会填充的上图中的**content**位置

3.  上图的default布局也可以再_layouts目录下找到：

![image.png](https://upload-images.jianshu.io/upload_images/13813710-ff856856eb08d5a1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


    实际上根目录下index.html运行后,home-page.html里面的代码内容会填充到上图中的**content**位置
    jekyll是将分散在各个目录下的html文件拼接起来运行。

4.  **[文章链接](https://link.jianshu.com?t=http%3A%2F%2Fjmcglone.com%2Fguides%2Fgithub-pages%2F)这里有篇讲的比较好的，跟着该文章里的操作，能让你更熟悉**

## **Jekyll 语法**

上一步大概讲解了下Jekyll的目录结构，现在我们讲解下部分jekyll的语法，也可去官方网站学习更详细**[官方链接](https://link.jianshu.com?t=http%3A%2F%2Fjekyllcn.com%2Fdocs%2Fhome%2F)**

因为常写博客和网站搭建，经常用到Jekyll和Markdown，备忘下常用语法。
# Markdown常用语法
Markdown 的优点如下：

1 纯文本，所以兼容性极强，可以用所有文本编辑器打开。
2 让你专注于文字而不是排版。
3 格式转换方便，Markdown 的文本你可以轻松转换为 html、电子书等。
4 Markdown 的标记语法有极好的可读性。

## 标题

这是最为常用的格式，在平时常用的的文本编辑器中大多是这样实现的：输入文本、选中文本、设置标题格式。

而在 Markdown 中，你只需要在文本前面加上 `#` 即可，同理、你还可以增加二级标题、三级标题、四级标题、五级标题和六级标题，总共六级，只需要增加 `#` 即可，标题字号相应降低。例如：

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题 

```

*注：`#` 和「一级标题」之间建议保留一个字符的空格，这是最标准的 Markdown 写法。*

*你可以你的编辑器中尝试输入这六级标题，可以参考下方的截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-46c9de182ac8b3c3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 列表

列表格式也很常用，在 Markdown 中，你只需要在文字前面加上 `-` 就可以了，例如：

```
- 文本1
- 文本2
- 文本3

```

如果你希望有序列表，
也可以在文字前面加上 `1.` `2.` `3.` 就可以了，例如：

```
1\. 文本1
2\. 文本2
3\. 文本3

```

*注：`-`、`1.`和文本之间要保留一个字符的空格。*

*列表案例截图如下：*

![](https://upload-images.jianshu.io/upload_images/13813710-cacc7581a600092b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


在 Markdown 中，插入链接不需要其他按钮，你只需要使用 `[显示文本](链接地址)` 这样的语法即可，例如：

```
[简书](http://www.jianshu.com)

```

在 Markdown 中，插入图片不需要其他按钮，你只需要使用这样`[](图片链接地址)` 的语法即可，例如：

```
![](http://upload-images.jianshu.io/upload_images/259-0ad0d0bfc1c608b6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

```

*注：插入图片的语法和链接的语法很像，只是前面多了一个 `！`。*

*插入链接和图片的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-4e9ad2e76bce721c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 引用

在我们写作的时候经常需要引用他人的文字，这个时候引用这个格式就很有必要了，在 Markdown 中，你只需要在你希望引用的文字前面加上 `>` 就好了，例如：

```
> 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

```

*注：`>` 和文本之间要保留一个字符的空格。*

最终显示的就是：

> 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

*引用的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-6d4a813c14bdced6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 粗体和斜体

Markdown 的粗体和斜体也非常简单，用两个 `*` 包含一段文本就是粗体的语法，用一个 `*` 包含一段文本就是斜体的语法。例如：

```
 *一盏灯*， 一片昏黄；**一简书**， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

```

最终显示的就是下文，其中「一盏灯」是斜体，「一简书」是粗体：

*一盏灯*， 一片昏黄；**一简书**， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

*粗体和斜体的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-5596c573dc7787f0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 代码引用

需要引用代码时，如果引用的语句只有一段，不分行，可以用 ` 将语句包起来。
如果引用的语句为多行，可以将```置于这段代码的首行和末行。
*代码引用的案例截图：*

![](https://upload-images.jianshu.io/upload_images/13813710-79c0c6de3c111cb9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 表格

相关代码：

```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```

显示效果：

| Tables | Are | Cool |
| --- | --- | --- |
| col 3 is | right-aligned | $1600 |
| col 2 is | centered | $12 |
| zebra stripes | are neat | $1 |

<p></p>
相关代码：

```
dog | bird | cat
----|------|----
foo | foo  | foo
bar | bar  | bar
baz | baz  | baz

```

显示效果：

| dog | bird | cat |
| --- | --- | --- |
| foo | foo | foo |
| bar | bar | bar |
| baz | baz | baz |

<p></p>

## 显示链接中带括号的图片

![][1]
[1]: [http://latex.codecogs.com/gif.latex](https://link.jianshu.com?t=http://latex.codecogs.com/gif.latex)?\prod%20(n_{i})+1

代码如下:

```
![][1]
[1]: http://latex.codecogs.com/gif.latex?\prod%20\(n_{i}\)+1
```

# Jekyll常用语法
## **Jekyll 目录结构**

jekyll目录结构主要包含如下目录：

> _posts 博客内容
> _pages 其他需要生成的网页，如About页
> _layouts 网页排版模板
> _includes 被模板包含的HTML片段，可在_config.yml中修改位置
> assets 辅助资源 css布局 js脚本 图片等
> _data 动态数据
> _sites 最终生成的静态网页
> _config.yml 网站的一些配置信息
> index.html 网站的入口

那么这些目录是如何运作的呢？

1.  我们打开根目录下的index.html可以看到：

    > —
    > layout: home-page
    > —
    > **html代码段**

2.  上面的home-page我们到_layouts目录下可以找到：

    ![image.png](https://upload-images.jianshu.io/upload_images/13813710-51cadf0bf21bbb6a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


    实际上根目录下index.html运行后是home-page里面的代码内容，1中**html代码段**会填充的上图中的**content**位置

3.  上图的default布局也可以再_layouts目录下找到：

![image.png](https://upload-images.jianshu.io/upload_images/13813710-ff856856eb08d5a1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


    实际上根目录下index.html运行后,home-page.html里面的代码内容会填充到上图中的**content**位置
    jekyll是将分散在各个目录下的html文件拼接起来运行。

4.  **[文章链接](https://link.jianshu.com?t=http%3A%2F%2Fjmcglone.com%2Fguides%2Fgithub-pages%2F)这里有篇讲的比较好的，跟着该文章里的操作，能让你更熟悉**

## **Jekyll 语法**

上一步大概讲解了下Jekyll的目录结构，现在我们讲解下部分jekyll的语法，也可去官方网站学习更详细**[官方链接](https://link.jianshu.com?t=http%3A%2F%2Fjekyllcn.com%2Fdocs%2Fhome%2F)**

1. **{**% for post in paginator.posts %**} {**% endfor %**}**表示一个for循环,百分号之间的语句为要执行的语句，该段代码表示分页输出文章，分页数量在_config.yml中配置，**注意：分页只在根目录下的index.html中有效**

1. **{** site.自定义字段名称 **}** 表示获取_config.yml里面的自定义字段名称的值


1. **{**% for post in site.posts limit:2  %**} {**% endfor %**}**循环输出 2 篇文章

1. **{**%  for post in site.posts offset:0 limit:2 %**}**循环输出最新2篇文章


1. **{**% for tag in post.tags  %**} {**% endfor %**}**输出该篇文章里的tag


1. **{**% if link.type == site.blog_1  %**} {**% endfor %**}**字符串比较


1. **{**% assign count = 0 %**}****{**% assign count = count | plus: 1 %**}**定义assign变量加1


1. **\{\{**post.content \| strip_html \| strip_newlines \| truncate: 100 **\}\}**获取文章摘要，取前100个字符


1. 2018-02-10-你要添加的描述.markdown，文章命名格式，否则识别不了


1. **\{\{** page.date \| date: '%Y, %b %d' **\}\}**输出文章日期


1. **\{\{**page.title**\}\}**输出文章标题


1. **{**% if post.jekyll %**}** 判断文章里的jekyll字段是否为true


1. **{**% if paginator.previous_page %**}**是否有上一页


1. **{**% if paginator.next_page %**}**是否有下一页


1. **\{\{** paginator.previous_page_path **\}\}**上一页url


1. **\{\{** paginator.next_page_path **\}\}**下一页url


1. **\{\{** post.url | prepend: site.baseurl **\}\}**要访问的文章的url



