---
title: "本地存储 + 线上获取：我的个人数据库建构路径"
alias: 
  - "本地存储 + 线上获取：我的个人数据库建构路径"
created-date: 2022-09-21T18:43:54+0800
type: Simpread
banner: "https://cdn.sspai.com/2021/11/17/365ff29b5ab274691d99b1417912aade.png "
banner_icon: 🔖
tag: 
idx: 1
---

# 本地存储 + 线上获取：我的个人数据库建构路径

> [!example]- [🧷内部链接](<http://localhost:7026/unread/1>) [🌐外部链接](<https://sspai.com/post/69972>)    
> URI:: [🧷](<http://localhost:7026/unread/1>) [🌐](<https://sspai.com/post/69972>) 
> intURI:: [🧷内部链接](<http://localhost:7026/reading/1>)

%%
> [!example]+ **Comments**  
> ```dataview
> TABLE 
>     WITHOUT ID
>     link(Source, dateformat(date(Source), "yyyy-MM-dd")) as Date___, 
>     regexreplace(rows.Comments,"^@@\[\[.+?\]\]\s","") as "Comments"
> FROM "journals"
> WHERE  contains(cmnt, this.file.name)
> FLATTEN cmnt as Comments
> WHERE contains(Comments, this.file.name)
> GROUP BY file.link as Source
> SORT rows.file.day desc
> ```
>  **Description**:: 这是个信息轰炸的时代，除了必要的信息过滤手段外，每个人都应该构建属于自己的个人知识库。
%%

> [!md] Metadata  
> **标题**:: [本地存储 + 线上获取：我的个人数据库建构路径](https://sspai.com/post/69972)  
> **日期**:: [[2022-09-21]]  

## Annotations


> [!srhl2] [[SR1@本地存储 + 线上获取：我的个人数据库建构路径|📄]] <mark style="background-color: #ffeb3b">Highlights</mark> [🧷](<http://localhost:7026/unread/1#id=1663757635024>) [🌐](<http://localhost:7026/reading/1#id=1663757635024>)   
> 这是个信息轰炸的时代，除了必要的信息过滤手段外，每个人都应该构建属于自己的个人知识库。
> ^sran-1663757635024

> [!srhl6] [[SR1@本地存储 + 线上获取：我的个人数据库建构路径|📄]] <mark style="background-color: #ffb7da">Highlights</mark> [🧷](<http://localhost:7026/unread/1#id=1663757593476>) [🌐](<http://localhost:7026/reading/1#id=1663757593476>)   
> ![](https://cdn.sspai.com/2021/11/17/02dcb3e22348318ab27890b2272242a6.png)
> ^sran-1663757593476

> [!srhl2] [[SR1@本地存储 + 线上获取：我的个人数据库建构路径|📄]] <mark style="background-color: #ffeb3b">Highlights</mark> [🧷](<http://localhost:7026/unread/1#id=1663757042487>) [🌐](<http://localhost:7026/reading/1#id=1663757042487>)   
> 到的可能是一个共性问题，也就是：我们自己的笔记究竟该如何处理才最方便、最有助于个人成长？不同的软件有不同的理念，有的服务注重开放性，能够与市面上的其他服务共通，便于定制自己的
> ^sran-1663757042487

> [!srhl2] [[SR1@本地存储 + 线上获取：我的个人数据库建构路径|📄]] <mark style="background-color: #ffeb3b">Highlights</mark> [🧷](<http://localhost:7026/unread/1#id=1663757046716>) [🌐](<http://localhost:7026/reading/1#id=1663757046716>)   
> 1.  究竟什么样的个人数据存储方案才是好的？
> 2.  如何构建适合自己的数据存储空间？
> 3.  构建自己的个性化服务应该注意哪些内容？
> ^sran-1663757046716

> [!srhl3] [[SR1@本地存储 + 线上获取：我的个人数据库建构路径|📄]] <mark style="background-color: #a2e9f2">Highlights</mark> [🧷](<http://localhost:7026/unread/1#id=1663757053676>) [🌐](<http://localhost:7026/reading/1#id=1663757053676>)   
> ![](https://cdn.sspai.com/2021/11/17/d603dfc12369401e5d24eeff2c2ddb85.jpg)
> ^sran-1663757053676

