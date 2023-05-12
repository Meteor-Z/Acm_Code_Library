# 使用Pandoc构建Acm模板

下周日打完河南ICPC省赛就要退役了，以后一场比赛前想要整理一下板子，想要一个拥有`目录`，`页眉`。`页脚`的Acm模板，这样就可以在比赛的时候快速翻阅，而且要更加好看

但是存在的问题是：很多构建 Acm模板的时候会使用`Latex`进行构建，但是我使用了很多，要么是些许麻烦，也许是我太笨了（呜呜呜qwq）,很多不能正常使用，我想要一种`简单`，`快捷`的构建Acm模板的方法，找了很多方法，最终使用了`pandoc`来构建Acm模板

这里我们只使用了Pandoc的一个基本的方法，使用`Pandoc`将`md`文件转换成`word`文件。

## 下载Pandoc

### windows

可以直接在网上进行搜索pandoc的安装包进行下载，但是在windows上我们可以使用一个更好用的包管理器`scoop`来安装`pandoc`，具体`scoop`的下载使用可以参考其他的教程qwq,,`pandoc`因为在`scoop`里面的`main`桶里面，所以可以直接这样进行安装

```sh
scoop install pandoc
```
稍等片刻就可以可以直接使用`pandoc`了，

### linux Mac

在`linux`和类Unix系统上有更加吧方便的包管理器，这里可以举例在`Arch Linux`上进行安装，

```sh
sudo pacman -S pandoc
```

### 转化成word文档

准备好md文档，可以直接使用命令来进行转换,在命令行上进行输入,建议Windows使用`Windows Terminal`和`Windows powershell`来配合使用
```sh
pandoc template.md -o template.docx
```

### 加入页眉，页脚，封面，目录

win上的office可以直接根据这个docx来增加页眉，页脚，封面，目录。具体按钮如下

插入选项中，依次选择增加页眉，页脚，封面，目录来进行排版，

### 导出成pdf

office左上角可以直接导出成pdf来进行保存，这样就完成了

具体成果可以访问github地址来查看效果

[github项目地址在此](https://github.com/Meteor-Z/Acm_Code_Library)  
[博客地址](https://www.cnblogs.com/Meteor-Z/)  
[知乎地址](https://www.zhihu.com/people/newlzc)