# 特点

这套工作流的特点：

1. 在阅读模式下加入稍后读，会自动生成本地快照
2. 在阅读模式下标注时，标注内容会自动同步到 Obsidian（轻量级使用简悦 + Obsidan）
3. 在 Obsidian 中也可以内嵌简悦的标注，同时也自动更新到 Obsidain 内的标注文档中（重度使用简悦 + Obsidan）

# 适合用户

- 新用户，尤其是需要使用简悦 + Obsidian 双链笔记配合的用户
- 不想折腾配置的用户

# 配置库文件说明

## 文件说明

- `Obsidian@simpread` → Obsidian 库文件，包含了跟简悦有关的一些插件
- `output` → 本地快照文件夹，内置了一些稍后读对应的本地快照
- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## Obsidian 库文件说明

内置了跟简悦有关系的四个插件：

- Banners
- Dataview
- Obsidian42 - BRAT
- SimpRead Sync

最主要的 SimpRead Sync 也配置完毕，内置了简悦的 Obsidain 模板，仅需要配置路径即可（下面的教程会告知如何配置）

## 内置 Obsidian 模板

内置了 https://github.com/Kenshin/simpread/discussions/2153#discussioncomment-2983977 基本上满足大部分 Obsidan 用户需求。

## 内置插件

### 阅读模式相关

- [题图](https://simpread.ksria.cn/plugins/details/PcmPCT9rgM)
- [模仿 Safari 阅读模式样式](https://simpread.ksria.cn/plugins/details/tbjTx33iAA)
- [Lightbox Gallery](https://simpread.ksria.cn/plugins/details/VQOZdNET2d)
- [Live Editor](https://simpread.ksria.cn/plugins/details/y8Mai5IBwN)

### 导入到 Obsidian 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [导入到 Obsidian](https://simpread.ksria.cn/plugins/details/1VQ19jCD8Z)
- [Markdown 模板辅助增强插件](https://simpread.ksria.cn/plugins/details/HD9GmoatXd)

以及 [插件管理器](https://simpread.ksria.cn/plugins/details/UEzvAXNSe5) 防止在开启同步助手后偶尔会出现无法正常安装插件的问题。（仅个别用户发生）

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 如果是新用户的话，请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx) 并且 [绑定了同步助手](https://www.yuque.com/kenshin/simpread/pwpnsx)
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

## 设置快照文件夹

也就是 `output` 文件夹，将下载的压缩包解压缩后放入到同步助手设置的同步盘文件夹。

![image-20220928092931084](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664328571.png)

如果你已经存在 `output` 文件夹的话，可以先将 `output` 文件夹改名为 `output@origin` 或其它名字。

## 设置 Obsidian 库文件夹

将解压缩的文件夹 `Obsidian@simpread` 放到你需要的任意目录，然后在 Obsidain 指定这个目录。

![image-20220928093550398](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664328950.png)

然后打开 SimpRead Sync 并按下图设定 `simpread_config.json` 的目录位置。

![image-20220928094417371](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664329457.png)

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

此配置包内置了9个插件。

![image-20220928104341346](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333021.png)

### 开启自动同步

使用此功能前，确保已经按照准备工作绑定了同步助手，选项页 → 共通 → 自动同步，开启下面的选项，并一定要选择 **通过简悦 · 同步助手覆盖本地配置文件**。

![image-20220928105621667](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333781.png)

然后刷新当前页面，即可生效。

上述完成后，此配置文件全部配置完毕。

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

###  在阅读模式下标注

然后再开启 Obsidain 的前提下，增加新的标注，看看是否会自动同步到 Obsidan。

<需要一个视频>

### 在 Obsidian 中标注

打开 Obsidan 里面应该有一些现成的 Markdown，打开一个并按照下面视频的操作，当在右侧标注时，会自动将标注同步到 Obsidian 中。

https://user-images.githubusercontent.com/81074/192680366-d7bd67a9-77da-4a04-ad83-f98d8e705962.mp4

https://user-images.githubusercontent.com/81074/192685660-35a6ae06-0c33-44ef-9208-0b806048059e.mp4

### 查看本地快照

打开稍后读，随便找一个已经存在的稍后读，如果有下面视频所示的标识则说明读取的本地文件。

https://user-images.githubusercontent.com/81074/192681150-f3986a9c-9983-4bae-b93b-768368b00bf5.mp4
