<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
        }
    });
</script>
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

# 前言

[TOC]

把学习到的知识全都总结、整理到这里，方便以后查阅、复习

## 本博客操作说明

### Latex语法和数学公式

公式行内公式和行间公式

- 行内公式：公式在一行文字之中，使用两个`$`夹住，例如`$x = 1$`
- 行间公式：公式单独一部分，占一些行



| 符号                                        | latex语法                    |
| :------------------------------------------ | :--------------------------- |
| 集合中的花括号`{}`                          | `\{ 元素1,元素2... }\`       |
| 集合中的花括号`{}`                          | 左括号\lbrace；右括号\rbrace |
| 集合中的竖线$\mid$                          | \mid                         |
| 集合中的属于$\in$                           | \in                          |
| 集合中的A包含于B(子集),$A\subset B$         | A\subset B​                   |
| 集合中的A真包含于B(真子集),$A\subsetneqq B$ | A\subsetneqq B​               |
| 集合中的A包含B,$A\supseteq B$               | A\supseteq B​                 |
| 集合中的A真包含B,$A\supsetneqq B$           | A\supsetneqq B               |
| 集合中的A不包含于B,$A\not\subset B$         | A\not\subset B               |
| 集合中的A交B,$A\cap B$                      | A\cap B                      |
| 集合中的A并B,$A\cup B$                      | A\cup B                      |
| 集合中的A的闭包,$\overline{A}$              | \overline{A}                 |
| 集合中的A减去B,$A\setminus B$               | A\setminus B                 |
| 集合中的实数集合$\mathbb{R}$                | \mathbb{R}                   |
| 集合中的空集$\emptyset$                     | \emptyset                    |
|                                             |                              |
| 三角形符号$\Delta ABC$                      | \Delta ABC                   |
| 绝对值$\vert x \vert$                       | \vert x \vert                |
| 角AOB$\angle AOB$                           | \angle AOB                   |
| 角度表示$0^\circ$                           | 0^\circ                      |
| 单向推导箭头$\Rightarrow$                   | \Rightarrow                  |
| 双向互推箭头$$\Longleftrightarrow$$         | \Longleftrightarrow​          |
| 双向互推箭头$\Leftrightarrow$               | \Leftrightarrow              |
| 垂直符号$\bot$                              | \bot                         |
|                                             |                              |
|                                             |                              |



#### 公式对齐

下面是不带左花括号形式

```
\begin{aligned}
&y=kx+b+222\\
&y=kx^2+b\\
\end{aligned}
```

$$
\begin{aligned}
&y=kx+b+222\\
&y=kx^2+b\\
\end{aligned}
$$

```
\begin{aligned}
y=kx+&b+222\\
y=kx^2+&b\\
\end{aligned}
```

$$
\begin{aligned}
y=kx+&b+222\\
y=kx^2+&b\\
\end{aligned}
$$

&标记的被对齐

### 

下面是带左花括号形式

```
\left\{
    \begin{array}{l}
            \dot{x_1} = x_2 \\ 
            \dot{x_2} = f(x_1,x_2) + bu \\
            y = x_1
        \end{array}
\right.          \tag{1}
```

$$
\left\{
    \begin{array}{l}
            \dot{x_1} = x_2 \\ 
            \dot{x_2} = f(x_1,x_2) + bu \\
            y = x_1
        \end{array}
\right.          \tag{1}
$$



#### 公式编号

```
\left\{\begin{matrix}
& \dot{x_1} = x_2 \\ 
& \dot{x_2} = f(x_1,x_2) + bu 
\end{matrix}\right.   \tag{1}
```

$$
\left\{\begin{matrix}
& \dot{x_1} = x_2 \\ 
& \dot{x_2} = f(x_1,x_2) + bu 
\end{matrix}\right.   \tag{1}
$$



































例如：

- $A = \lbrace x\mid f(x) = 0\rbrace$的代码如下：

  ```
  $A = \lbrace x\mid f(x) = 0\rbrace$
  ```


行间公式：快捷键为`shift+ctrl+m`，需要在公式前后加回车换行，否则显示可能不正常，使用Latex在线编辑器编辑即可。


$$
\left\{\begin{array}{l}  \dot{x_{1}}=x_{2}
\\ \dot{x_{2}}=f(x_{1},x_{2})+bu
\\ y=x_{1}
\end{array}\right.
$$

代码如下：

```
\left\{\begin{array}{l}  \dot{x_{1}}=x_{2}
\\ \dot{x_{2}}=f(x_{1},x_{2})+bu
\\ y=x_{1}
\end{array}\right.
```



### 本博客主题

本博客使用Github提供的github page，和[jekyll主题模版](http://jekyllthemes.org/)配合使用，步骤如下：

**1. 注册 Github 账号，安装登陆github desktop**

**2. 在 Github 上创建仓库并且设置**

网页创建仓库、同步仓库到本地、网页进入仓库、选择Setting，设置GitHub Pages（main、root）、把主题模板复制到本地仓库根目录，同步上去即可

**3. 打开博客**

在Setting中的GitHub Pages下，可以看到链接，其实就是仓库的地址。为了方便仓库的名字可以设置为：Github用户名.github.io。我的仓库名是`life696.github.io`，我的链接是`https://life696.github.io/`



### 字体

<center>这是要居中的文本内容</center>

---

分割线：三个---或者***，回车换行

---

_斜体：下划线夹住_、~~横线：双波浪号~~、`内联代码：灰色背景、红色字体，快捷键：shift+ctrl+反单引号(tab键上面的键)`、[链接：中括号和圆括号](https://www.baidu.com/)、__粗体：双下划线夹住或者双星号夹住，快捷键ctrl+B__



{:.text-red}

红色字体、默认背景，直到换行结束，只管一段。

{:.bg-yellow-dark}
默认颜色、有背景，直到换行结束，只管一段

{:.bg-yellow-dark.text-white.p-2.box-shadow-large}

大边框背景色

{:.bg-yellow-dark.text-white}
有背景、有颜色，直到换行结束，只管一段

{:.bg-yellow-dark.text-white.m-5}

有背景、有颜色，字和背景都缩进

{:.bg-yellow-dark.text-white.p-5.mb-6}
有背景，有颜色，段落有缩进，但背景色不缩进

{:.bg-yellow-dark.text-white}
某些字符加**大**{:.h1}



```tip
这是一个tip
```

```note
这个是note
```



### 图片引用

格式`![名字](图片路径)`，直接截图复制到markdown 文档即可，markdown设置为如果有图片复制进来，就在这个文件的同级目录创建`这个文件名字_img`的文件夹，图片自动放进来，但是如果在文档中把图片删除，文件夹中的图片依然在，需要手动删除

网络图片也可以修改大小，右键修改如下：

```
<img src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=3832721317,312397218&fm=26&gp=0.jpg" alt="avatar" style="zoom: 80%;" />
```

<img src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=3832721317,312397218&fm=26&gp=0.jpg" alt="avatar" style="zoom: 80%;" />

本地图片，也可以自定义图片的位置和大小

```
<div align="center"><img width="600" height="auto" src="preface_img/1.jpg"/></div>
```



<div align="center"><img width="600" height="auto" src="preface_img/1.jpg"/></div>



Github仓库上的图片，加载的速度还可以，但是手机端不显示...还是使用本地方式保存吧，然后一起上传到云仓库

<img width="600" height="auto" src="https://raw.githubusercontent.com/life696/images/master/img1/4.jpeg"/>







### 插入代码

```
快捷键：shift+ctrl+k
然后右下角选择语言种类
```



### 插入引用快

> 这是引用块
>
> 快捷键：shift+ctrl+q



### 页内跳转（页内目录）

Github Pages中不显示markdown的目录，只能自己实现，如下：

- 点击此处就跳转： `[跳转到某个标题](#我是某个标题)`  
- 目标位置：`我是某个标题`

注意：目标位置必须是有等级的目录

### HTML语法

使用`span`或者`font`标签，同时用`style`属性控制样式。

<font face="微软雅黑" color="red" size="6">1.字体及字体颜色和大小，代码如下：</font>

```
<font face="微软雅黑" color="red" size="6">1.字体及字体颜色和大小，代码如下：</font>
```

<font color="#0000ff">2.字体颜色，代码如下：</font>

```
<font color="#0000ff">2.字体颜色</font>
```

<span style='color:red'>3.This is red</span> 

```
<span style='color:red'>3.This is red</span> 
```

4.按键标识<kbd>Ctrl</kbd>+<kbd>F9</kbd>

```
<kbd>Ctrl</kbd>+<kbd>F9</kbd>
```

<span style="font-size:2rem; background:yellow;">5.字体大小和背景</span> 

```
<span style="font-size:2rem; background:yellow;">5.字体大小和背景</span> 
```

<p align="left">6.居左文本，代码如下</p>

```
<p align="left">6.居左文本</p>
```

<p align="center">7.居中文本，代码如下</p>

```
<p align="center">7.居中文本</p>
```

<p align="right">8.居右文本，代码如下：</p>

```
<p align="right">8.居右文本</p>
```



### 行距

在Typora中shift + enter是单回车（间距小），而enter是双回车（间距大）。

但是在网页中只有双回车才是真的回车换行

### 相关修改

**1. 修改了_includes\templates\addons.liquid**

删除`addons.liquid`和`addons.scss`，删除左边栏最下面的小窗口

**2. 修改了_includes\templates\footer.liquid**

修改了底部内容

### 可能存在的问题

**1. latex公式问题**

jekll不支持latex公式，在`_include文件夹`中搜索`head`，可以找到一个`head.html`文件，记事本打开，里面没有内容，加入如下内容：

```
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
        }
    });
</script>
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
```



**2. 网页Github-Setting报错问题**

报错信息为：

GitHub Pages
GitHub Pages is designed to host your personal, organization, or project pages from a GitHub repository.

 The CNAME jekyll-rtd-theme.rundocs.io is already taken. Check out https://docs.github.com/articles/troubleshooting-custom-domains#cname-errors for more information.

解决：

找到根目录下的CNAME文件，删除。

或者有其他报错问题，遇到再修改！**要保证：**每提交一次修改，最后都要在github-setting中看是否有错误。

## Git命令

安装git工具软件，该软件为`Git-2.26.2-64-bit.exe`

### 1. 安装软件之后，连接github账户

- 鼠标右键单击，选择`Git GUI Here`

- 点击菜单栏`Help`，选择`Show SSH Key`

- 点击右上角`Generate Key`，把代码复制

- 在GitHub网页创建仓库，点击用户账号头像下的`Setting`

- 选择左侧的`SSH and GPG keys`

- 在`SSH keys`部分点击`New SSH key`，把在`Generate Key`复制的代码，粘贴到这里，点击`Add SSH key`

- 选择一个合适的目录（文件夹），在这里右键打开`Git Bash Here`，输入如下代码：

  ```
  git config --global user.name "用户名"
  ```

  ```
  git config --global user.email "邮箱"
  ```

### 2. 克隆云端仓库到本地

克隆云端仓库，如果是空仓库，进入就会看到链接。如果不是空仓库，就点击`Code`，下面就会弹出链接

```
git clone https://github.com/life696/life696.github.io.git
git clone git@github.com:life696/life696.github.io.git
```

以上两条选择一个，`https`的不行，就用`SSH`的

### 3. 本地的修改文件后，推送到云端

三合一直接推送到云端：`git add . && git commit -m "更新" && git push origin master`

添加修改的文件：

- 添加某个文件：`git add a.c`   
- 添加所有文件：`git add .`  

提交本次修改信息：`git commit -m "备注信息"`

上传到云仓库master分支：`git push origin master`

查看是否还有未提交的：`git status`

```
$ git status
On branch master
Your branch is based on 'origin/master', but the upstream is gone.
(use "git branch --unset-upstream" to fixup)

nothing to commit, working tree clean
```



### 4. 清理本地.git文件夹

随着提交版本次数越多，本地`.git`文件夹就会越来越大，这个文件夹中，因为保存了大量的历史版本。例如有如下操作：

- 第一次：上传了100张图片（10M）
- 第二次：删除了100张图片，并且重新换了100张图片（11M），又新增了100张图片（12M）

那么现在`.git`中有第一次和第二次的版本数据，现在有10+11+12=33M的数据，而第一次中的10M，是不需要的

了（有时候可能需要，有时是真的不需要了）我们需要删除他们。

```note
为什么要删除他们呢？
0. 必须是确保他们是不需要的文件，并且有删除的必要
1. 占用本地太大，不方便灵活，而且不知道版本数据会不会在仓库限制的1G之内（我不知道，所以还是删了吧）
2. 即使是删除的文件，也要确保备份（网盘、移动硬盘等等）
```



删除历史commit数据，有两种方案：

- 方案一：直接删除.git文件夹，重新构建仓库，强制推送（亲测有效，但如果文件较多，会很慢）
- 方案二：清楚本地所有commit记录，然后重新推送到云端（亲测失败，云端commit记录清空，本地仍在。不知道为什么，先做记录，以后再查）



**方案一：重新构建仓库（有效）**

大体步骤如下：

- 删除本地`.git`文件夹：`rm -rf .git`

- 重新构建本地仓库：`git init`

- 添加所有文件：`git add .`

- 提交：`git commit -m "reinit"`

- 强制推送：`git push -f -u origin master`，需要注意的是，此步可能报错推不上去，解决如下：

  ```note
  报错信息：
  fatal: 'origin' does not appear to be a git repository
  fatal: Could not read from remote repository.
  Please make sure you have the correct access rights and the repository exists
   
  ```

  - 与远端连接（姑且这叫）：`git remote add origin 项目地址`
  - 重新推送：`git push -f -u origin master`

总结一下就是：

- 删除本地commit并且重构从库，重新commit：

  `rm -rf .git && git init && git add . && git commit -m "reinit"`

- 强制推送：

  `git remote add origin 你的项目地址 && git push -f -u origin master`

  



**方案二：清除commit记录**

大致流程如下：

- 切换分支：`git checkout --orphan latest_branch`
- 添加到暂存区：`git add -A`
- 提交更改： `git commit -am "to init"`
- 删除分支： `git branch -D master`
- 重命名分支： `git branch -m master`
- 强制提交到远程仓库：`git push -f origin master`



















## 链接汇总

### 书画篆刻

[中国历代书法名家作品全集](http://www.sfzj123.com/person/getPersons?pt=01)   |   [欧阳询楷书基本笔画正确写法](http://www.360doc.com/content/19/0225/12/18577042_817404443.shtml)  |  [宋拓《九成宫醴泉铭》高清整碑复原版](https://www.sohu.com/a/155103304_258370)     |    [李祺藏本高清](https://m.wang1314.com/doc/webapp/topic/21056376.html)    |    [宋拓-高凤翰等递藏本](http://www.360doc.com/content/18/0511/00/9598567_752869594.shtml)     |    [三井本、姚孟起临本](http://www.360doc.com/content/20/0409/18/10243616_904897413.shtml)    |    [田蕴章临九成宫](http://www.360doc.cn/mip/822353785.html)    |    [蜀素帖](https://baijiahao.baidu.com/s?id=1655508851450404227&wfr=spider&for=pc)    |    [四时读书乐](https://mp.weixin.qq.com/s?__biz=MzUxMzUzMDc4Mg==&mid=2247496859&idx=3&sn=f76df03dbb326ad8a028da36c742987c&chksm=f9517a6ace26f37c3f408e0d19501bc700e41f13ac14e29c545c6220a6bb68b9ca465ba2bed7&scene=126&sessionid=1594819948&key=3a7b1476f26f2484c6c19988200ad562ca94e6c6f3b5120a80c8bc4a3b99a505bb4ba474b3b611c09d4ec8104e152263cadcbd742338960e20702914b9c68deae1bb5b8de041b551932e2d46c8be574f&ascene=1&uin=NTk2NTIxMTc2&devicetype=Windows+7+x64&version=6209007b&lang=zh_CN&exportkey=A1IorssFKVOZhL0i7oQtfM8%3D&pass_ticket=%2FDAWp8T9EwPuNPsl7iKmM537ZmSKt%2Fu0IYABkBYhk4alihG%2FgugQdNsL4w%2FOEZL4)    |    [值得临写的篆书](http://www.360doc.com/content/19/0629/16/16556281_845600138.shtml)    |    [碑文高清大图及技法学习](http://www.360doc.com/content/19/0623/18/15521688_844371161.shtml)    |    [李斯简介及诗文](https://www.gushiwen.org/Author_aa21e3aa6f.aspx)     |    [为什么选择皇甫诞](https://www.sohu.com/a/214894794_131728)    |    [高清大字三门记](https://www.sohu.com/a/220295756_657937)     |    [前后赤壁赋笔法](https://www.sohu.com/a/190895059_469206)



### 嵌入式技术

[正点原子资料下载中心](http://www.openedv.com/docs/index.html#)     |    [linux 5.11 内核文档](https://www.kernel.org/doc/html/latest/index.html)    |    [Linux内核代码风格](https://www.kernel.org/doc/html/latest/translations/zh_CN/process/coding-style.html)    |    [百问网资料中心](http://download.100ask.net/index.html)    |    [操作系统学习](https://rcore-os.github.io/rCore-Tutorial-Book-v3/#)    |  [Think Python 2e](https://codingpy.com/books/thinkpython2/index.html)

### 学术理论

[蒲慕明：博士研究生如何做创新性研究](http://www.360doc.com/content/19/0407/10/7151997_826951162.shtml)



## 要整理的内容

- 傅里叶变换
- 拉氏变换
- Z变换
- 级数展开
- 什么是模块化编程？如何实现？
- 




