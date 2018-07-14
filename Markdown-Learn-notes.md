---
title: "Markdown Learn Notes"
date: 2018-07-03T19:48:42+08:00
draft: false
---
- wei
- he
- bu
- ke
- 之所以会显示前一行是因为我在中括号前加了反斜杠（转义字符）

> 我搞了个空行后面才可以在Hugo中显示项目黑点和注释，但在Atom编辑器预览中不用空行就可以

## 插入超链接
超链接的语法为:  

      \[超链接的说明性内容](超链接)    

方括号内是这个超链接的说明性内容（自己随便写），甚至可以是一个图片（即为图片添加超链接）  

>出现上面的方框是因为我把前后都空一行，并且方框内文本所在的那一行行首加了四个空格

例如:在.md文件中输入

    \[谷歌](http://www.google.com/)

则在生成文件中效果为：
[谷歌](http://www.google.com/)  


- 之所以会显示前一行是因为我在中括号前加了反斜杠（转义字符）
## 插入图片  
插入图片只需在方括号前再加一个叹号，例如

      \!\[本地图片](./图片/notations.png)

效果为插入一张在当前文件夹下图片子文件夹的notations.png图片（如果这张图片存在的话）
![本地图片](./图片/notations.png)