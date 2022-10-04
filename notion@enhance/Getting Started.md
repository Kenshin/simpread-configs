<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221003_1664782925.png" /></p>

# 特点

1. 导入到 Notion 时会将图片上传到 Notion （也就是开启 Notion 图床功能），防止图片 404
2. 在阅读模式下加入稍后读，会将正文导入以 Markdown 的格式导入到 Notion
3. 在阅读模式下标注时，标注内容会自动同步到 Notion
4. 不使用同步助手，非常适合轻量级使用简悦 + Notion 的用户

# 适合用户

- 新用户，尤其是需要使用简悦 + Notion 双链笔记配合的用户
- 不想折腾配置的用户

# 配置库文件说明

## 内置 Notion 账户

为了更直观的看到通过简悦导入到 Notion 后的效果，配置文件包含了简悦官方提供的 Notion 授权信息。

使用 `zaqr7s0g7@mozmail.com / sr123_654` 登录到 Notion 后可直接使用。

**注意**

1. 不要修改测试账户的密码，我会随时找回。😂
2. 测试账户只是让新用户更直观的看到通过简悦的导入效果，最终还是要更换为自己的账户。
3. 如何使用请看下面的附录内容。

## 文件说明

- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## 内置插件

### 阅读模式相关

- [题图](https://simpread.ksria.cn/plugins/details/PcmPCT9rgM)
- [模仿 Safari 阅读模式样式](https://simpread.ksria.cn/plugins/details/tbjTx33iAA)
- [Lightbox Gallery](https://simpread.ksria.cn/plugins/details/VQOZdNET2d)
- [Live Editor](https://simpread.ksria.cn/plugins/details/y8Mai5IBwN)

### 导入到 Obsidian 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [导入到 Notion 辅助增强](https://simpread.ksria.cn/plugins/details/g60jwZEeqU)

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 如果是新用户的话，请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx)。
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

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

此配置包内置了8个插件，导入成功后会有下图所示的提示。

![image-20221001184549812](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221001_1664621149.png)

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

###  在阅读模式下加入稍后读和标注

https://user-images.githubusercontent.com/81074/193757575-49c4cc2a-2df9-406b-a683-b409d6555009.mp4

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## 更换自己的 Notion 账户

## 合并稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20220929185850419](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449130.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20220929190305838](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449385.png)
