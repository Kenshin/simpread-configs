<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221008_1665202307.png" /></p>

# 特点

1. 在阅读模式下加入稍后读，会自动生成本地快照
2. 在阅读模式下加入稍后读，会自动以 md + assets 方案保存到本地，解决图片 404 的问题
3. 在阅读模式下标注时，标注自动生成本地快照

# 适合用户

- 不想折腾配置的用户
- 喜欢使用 HTML 作为网页永久化保存的用户

# 配置库文件说明

## 文件说明

- `output` → 本地快照文件夹，内置了一些稍后读对应的本地快照
- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## 内置插件

### 阅读模式相关

- [题图](https://simpread.ksria.cn/plugins/details/PcmPCT9rgM)
- [模仿 Safari 阅读模式样式](https://simpread.ksria.cn/plugins/details/tbjTx33iAA)
- [Lightbox Gallery](https://simpread.ksria.cn/plugins/details/VQOZdNET2d)
- [Live Editor](https://simpread.ksria.cn/plugins/details/y8Mai5IBwN)

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)

### assets + md 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [导出 md + assets 格式](https://simpread.ksria.cn/plugins/details/BvjrJA6eh5)

以及 [插件管理器](https://simpread.ksria.cn/plugins/details/UEzvAXNSe5) 防止在开启同步助手后偶尔会出现无法正常安装插件的问题。（仅个别用户发生）

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 如果是新用户的话，请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx) 并且 [绑定了同步助手](https://www.yuque.com/kenshin/simpread/pwpnsx)。
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

## 设置快照文件夹

也就是 `output` 文件夹，将下载的压缩包解压缩后放入到同步助手设置的同步盘文件夹。

![image-20220928092931084](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664328571.png)

如果你已经存在 `output` 文件夹的话，可以先将 `output` 文件夹改名为 `output@origin` 或其它名字。

如果没有 `Output` 文件夹的话，在设置的同步文件夹下新建 `output` 即可，并在同步助手 → 导出 → 路径，添加 `output` 路径。

![image-20221006165001158](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221006_1665046201.png)

## 设置 md + assets 位置

![image-20221009161643869](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221009_1665303403.png)

当生成后 文件后自动生成到 `xxx` 文件夹，我一般都是保存到 Obsidian 对应的文件夹

```
{"extension":"assets", "path":"/Users/xxxx/Obsidian@simpread"}
```

如果是 Windows 系统的话，请使用下面的方案（留意有两个斜杠 `\\`）

```
{"extension":"assets", "path":"C:\\Users\\***\\Obsidian@simpread"}
```

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

此配置包内置了6个插件，导入成功后会有下图所示的提示。

![image-20221005120248874](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664942568.png)

### 开启自动同步

使用此功能前，确保已经按照准备工作绑定了同步助手，选项页 → 共通 → 自动同步，开启下面的选项，并一定要选择 **通过简悦 · 同步助手覆盖本地配置文件**。

![image-20220928105621667](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333781.png)

然后刷新当前页面，然后会在你的同步助手设置的同步文件夹下发现 `simprea_config.json` 文件，即说明导入成功。

![image-20220929184021771](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664448021.png)

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

### 加入稍后读自动生成 md + asset 格式

https://user-images.githubusercontent.com/81074/194745998-52f38bad-617c-49b1-88c1-f561ad756d3b.mp4

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