<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665118121.png" /></p>

# 下载地址

[Github](https://github.com/Kenshin/simpread-configs/releases) 或 [百度云](https://pan.baidu.com/s/1SkFLJ21CKFL4lhWPhEg0iA?pwd=99mq) 请下载 `logseq@md.zip` 

# 特点

1. 在阅读模式下加入稍后读，会自动生成本地快照
2. 在阅读模式下标注时，标注内容会自动同步到 Logseq
3. 在 Logseq 中也可以内嵌简悦的标注，同时也自动更新到 Logseq 内的标注文档中

# 适合用户

- 新用户，尤其是需要使用简悦 + Logseq 双链笔记配合的用户
- 不想折腾配置的用户

# 配置库文件说明

## 文件说明

- `Logseq@simpread` → Logseq 库文件，包含了跟简悦有关的一些插件
- `.logseq` → SimpRead Sync 插件
- `output` → 本地快照文件夹，内置了一些稍后读对应的本地快照
- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## Logseq 库文件说明

- [SimpRead Sync](https://github.com/OverflowCat/logseq-simpread)

## 内置 Logseq 模板

内置了 https://github.com/Kenshin/simpread/discussions/2153#discussioncomment-2627320 基本上满足大部分 Logseq 用户需求。

## 内置插件

### 阅读模式相关

- [题图](https://simpread.ksria.cn/plugins/details/PcmPCT9rgM)
- [模仿 Safari 阅读模式样式](https://simpread.ksria.cn/plugins/details/tbjTx33iAA)
- [Lightbox Gallery](https://simpread.ksria.cn/plugins/details/VQOZdNET2d)
- [Live Editor](https://simpread.ksria.cn/plugins/details/y8Mai5IBwN)

### 导入到 Logseq 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [将标注以 Markdown 2.0 模板形式导出](https://simpread.ksria.cn/plugins/details/8jnsO2OtHW)
- [Markdown 模板辅助增强插件](https://simpread.ksria.cn/plugins/details/HD9GmoatXd)

以及 [插件管理器](https://simpread.ksria.cn/plugins/details/UEzvAXNSe5) 防止在开启同步助手后偶尔会出现无法正常安装插件的问题。（仅个别用户发生）

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx) 并且 [绑定了同步助手](https://www.yuque.com/kenshin/simpread/pwpnsx)。
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

## 设置快照文件夹

也就是 `output` 文件夹，将下载的压缩包解压缩后放入到同步助手设置的同步盘文件夹。

![image-20220928092931084](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664328571.png)

如果你已经存在 `output` 文件夹的话，可以先将 `output` 文件夹改名为 `output@origin` 或其它名字。

如果没有 `Output` 文件夹的话，在设置的同步文件夹下新建 `output` 即可，并在同步助手 → 导出 → 路径，添加 `output` 路径。

![image-20221006165001158](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665046201.png)

## 设置 Logseq 库文件夹

将解压缩的文件夹 `Logseq@simpread` 放到你需要的任意目录，然后在 Logseq 指定这个目录。

![image-20221006155135282](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665042695.png)

## 设置 .md 导出位置

在同步助手 → 导出中按下图所示设置。

![image-20221007114713784](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665114433.png)

当生成 `.md` 文件后自动生成到 `Logseq@simpread` 文件夹。

```
{"extension":"md", "path":"/Users/xxxx/Logseq@simpread/pages"}
```

如果是 Windows 系统的话，请使用下面的方案（留意有两个斜杠 `\\`）

```
{"extension":"md", "path":"C:\\Users\\***\\Logseq@simpread\\pages"}
```

## 设置 Logseq 文件格式

在选项中要确保是 `.md` 格式。

![image-20221007114819904](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665114499.png)

## 导入 .logseq 文件夹

### 自动安装

打开 Logseq 的插件市场，输入 `simpread` 然后安装即可。

![image-20221006160411926](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665043451.png)

没有插件市场的话，请通过下图所示的方式开启。

![image-20221006191310436](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665054790.png)

### 手动安装

Logseq 与 Obsidian 的插件机制不一样，Logseq 属于全局，所以没法跟 Obsidian 一样直接复制库文件夹即可，下面以 Logseq 为例说明。

打开解压缩后的 `.logseq` 文件夹，会得到下面的结构

![image-20221006160108761](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665043268.png)

打开 `/Users/xxx/.logseq` （ `xxx` 为自己的在 Mac 上的名字 ），将上图的内容复制到下图所示的位置。

![image-20221006162713512](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665044833.png)

### 验证

无论哪种方式，进入 Logseq 后，如果有下图所示的 Icon 则说明安装成功。

![image-20221006155308565](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665042788.png)

## 导入配置文件

### 复制 UID

在选项页 → 账户 → 用户信息处复制你的 UID 到剪切板。（接下来的步骤会使用）

![image-20220928102913588](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664332153.png)

### 导入

建议使用一个新的浏览器或者在留存当前配置文件的前提下，重新安装简悦。安装完简悦后，通过选项页 → 共通 → 从本地导入配置文件到。

![image-20220928103241097](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664332361.png)

### 恢复高级账户资格

导入并刷新后，进入账户 → 用户信息，修改为你自己的高级账户 UID（也就是在准备阶段让你复制的 UID）

![image-20220928103642338](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664332602.png)

保存后根据提示信息操作即可恢复你的高级账户资格。

![image-20220928103930520](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664332770.png)

### 导入插件

因为插件都比较大，因此并不包含在配置文件中，配置文件仅包含了插件的配置信息，因此导入新的配置文件后还需要导入插件，位置在：选项页 → 插件管理 → 从配置文件导入插件。

![image-20220928104247433](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664332967.png)

此配置包内置了9个插件，导入成功后会有下图所示的提示。

![image-20220928104341346](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333021.png)

### 开启自动同步

使用此功能前，确保已经按照准备工作绑定了同步助手，选项页 → 共通 → 自动同步，开启下面的选项，并一定要选择 **通过简悦 · 同步助手覆盖本地配置文件**。

![image-20220928105621667](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333781.png)

然后刷新当前页面，然后会在你的同步助手设置的同步文件夹下发现 `simprea_config.json` 文件，即说明导入成功。

![image-20220929184021771](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664448021.png)

## 设置模板

打开 `http://localhost:7026/unread/1?embed=logseq`  ，如果上述步骤无误的话，会出现下图所示的内容。

![image-20221006160759134](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665043679.png)

打开左上角 Icon，并按照下图所示设置。

![image-20221007115230775](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665114750.png)

### 稍后读模板

```
title:: {{title}}
host:: {{host}}
type:: Simpread
tags:: {{tags}}
date:: [[{{create|yyyy年mm月dd日}}]]

<% if ( unread.desc ) { %>
# 描述
> <%- unread.desc %>
<% } %>
<% if ( unread.refs ) { -%>
> 外部引用: {{refs}}
<% } %>
<% if ( unread.backlinks ) { -%>
> 反向连结: {{backlinks}}
<% } %>
<% if ( unread.annotations.length > 0 ) { -%>
# Annotations
{{annotations}}
<% } -%>
```

### 标注模板

```
<%
let colors = [ '#B4D9FB', '#ffeb3b', '#a2e9f2', '#a1e0ff', '#a8ea68', '#ffb7da' ],
    color  = colors[ annote.color ];
let url    = 'http://localhost:7026/unread/' + unread.idx + '#id=' + annote.id;
%>
## [📌](<<%= url %>>) Highlights {{an_tags}}
> [:p {:style {:background-color "<%= color %>"}} "{{an_text}}"]
<% if (annote.note) { %>
>> {{an_note}}
<% } %>
### reference
<%- (annote.refs)? "> refs: " + annote.refs : "" %>

> backlinks: {{an_backlinks}}

```

复制时请留意空格，复制粘贴保存后，刷新当前页面确保生效。上面的模板来自 https://github.com/Kenshin/simpread/discussions/2153#discussioncomment-3819505 关于 Logseq 的更多官方模式，[请看这里](https://github.com/Kenshin/simpread/discussions/3725#discussioncomment-2635600)。

上述完成后，此配置文件全部配置完毕。

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

###  在阅读模式下标注

然后再开启 Logseq 的前提下，增加新的标注，看看是否会自动同步到 Logseq。

https://user-images.githubusercontent.com/81074/194466873-e15cfba6-bc71-43da-b654-71af7d622656.mp4

### 在 Logseq 中标注

当在右侧标注时，会自动将标注同步到 Logseq 中。

https://user-images.githubusercontent.com/81074/194467146-9f466e47-bb86-4cdc-bb53-5e6d7e08641a.mp4

### 查看本地快照

打开稍后读，随便找一个已经存在的稍后读，如果有下面视频所示的标识则说明读取的本地文件。

https://user-images.githubusercontent.com/81074/192681150-f3986a9c-9983-4bae-b93b-768368b00bf5.mp4

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## 合并 output 和稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20220929185850419](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449130.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20220929190305838](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449385.png)

然后把配置库中 `output` 文件夹对应的快照 id 也对应修改下。

![image-20220929190542971](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449543.png)

以及 `Logseq@simpread/SimpRead`文件夹对应的快照 id。

## 阅读模式优化

当前配置包没有开启 **如果当前页面为适配站点，自动进入阅读模式** 的功能，如果需要开启请进入选项页 → 阅读模式，按下图所示开启。

![image-20221013091327937](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221013_1665623607.png)

当前配置库仅配置了少数派的白名单，例如进入 https://sspai.com/post/69972 后会自动进入阅读模式，白名单的位置在选项页 → 全局 → 白名单

![image-20221013091625016](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221013_1665623785.png)

简悦拥有多种自动进入阅读模式或聚焦模式的方案，包括：

- [使用白名单让任意页面实现【自动进入阅读模式】](https://github.com/Kenshin/simpread/discussions/1672)
- [当阅读模式并未符合你的期望时，如何进一步优化？](https://github.com/Kenshin/simpread/discussions/1554)
- [白名单](URL编辑器?id=白名单)、[黑名单](http://ksria.com/simpread/docs/#/URL编辑器?id=黑名单)、[排除列表](http://ksria.com/simpread/docs/#/URL编辑器?id=排除列表)、[延迟加载列表](http://ksria.com/simpread/docs/#/词法分析引擎?id=延迟加载) 的使用说明

更多关于阅读模式的技巧 [请看这里](https://github.com/Kenshin/simpread/discussions?discussions_q=label%3A%22read+mode%22)。