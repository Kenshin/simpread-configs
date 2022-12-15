<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221128_1669633812.png" /></p>

# 下载地址
[Github](https://github.com/Kenshin/simpread-configs/releases) 或 [百度云](https://pan.baidu.com/s/1SkFLJ21CKFL4lhWPhEg0iA?pwd=99mq) 请下载 `flowus@little.zip`

# 特点

1. 在阅读模式下加入稍后读，会将正文导入以 Markdown 的格式导入到 FlowUs
2. 不使用同步助手，非常适合轻量级使用简悦 + FlowUs 的用户
3. 适配 FlowUs 的分享页（可通过此方式进入阅读模式并导入到自己的 FlowUs 账户）

# 适合用户

- 新用户，尤其是需要使用简悦 + FlowUs 笔记配合的用户
- 不想折腾配置的用户

# 视频演示

[B 站视频](https://www.bilibili.com/video/BV1MP4y1Q7iE/) | [知乎视频](https://www.zhihu.com/zvideo/1586342219220520960)

https://user-images.githubusercontent.com/81074/207801259-0616a4ef-ab0a-4062-b8aa-1622184f3958.mp4

# 配置库文件说明

## 文件说明

- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## 内置插件

### 阅读模式相关

- [题图](https://simpread.ksria.cn/plugins/details/PcmPCT9rgM)
- [模仿 Safari 阅读模式样式](https://simpread.ksria.cn/plugins/details/tbjTx33iAA)
- [Lightbox Gallery](https://simpread.ksria.cn/plugins/details/VQOZdNET2d)
- [Live Editor](https://simpread.ksria.cn/plugins/details/y8Mai5IBwN)
- [Assistive Touch - 类似 iOS 的快捷浮动工具栏](https://simpread.ksria.cn/plugins/details/rsd4UIcDKY)

### 导入到 FlowUs 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [导入到 FlowUs](https://simpread.ksria.cn/plugins/details/NgDkX2TqAx)

### 内置适配规则

除了导入到 FlowUs 外，简悦还适配了 [FlowUs Page](https://simpread.ksria.cn/sites/details/cAlgLD4Qxb) 并内置到配置库中。

![image.png](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221128_1669634062.png)

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

### 登录并设置 FlowUs 授权

打开 [https://flowus.cn](https://flowus.cn/) 并登录你的 FlowUs 账户，打开 https://sspai.com/post/69972 并进入阅读模式 → 右下角 → 动作 → 插件触发器 → 导入到 FlowUs 选项，跟然后进行授权操作，并选择保存的 Page。

https://user-images.githubusercontent.com/81074/204266517-93520cd3-1c3d-4b5e-b890-56a3dac34b13.mp4

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

### 导入到 FlowUs

https://user-images.githubusercontent.com/81074/204264655-f468d490-ef67-4843-89d1-19fe19f3618b.mp4

### 加入稍后读后自动导入

https://user-images.githubusercontent.com/81074/204264699-71dae763-8223-48af-8533-c5117e84d9fd.mp4

### 适配 FlowUs 阅读模式

https://user-images.githubusercontent.com/81074/204264738-d5f4021f-a848-4a18-9d23-21b52bc35ab4.mp4

# 注意事项

- 使用此配置库方案**仅在阅读模式下使用**，在稍后读内置的阅读模式下无法使用。

- 使用此配置库方案**加入稍后读时只能使用快捷键** `d d` **或右键菜单的方式**，其它方式无法实现自动化。

  ![image.png](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221128_1669634437.png)

- 建议不要删除已经存在的示例稍后读，当删除全部稍后读后，第一个稍后读会没有标号。（细节请看 https://www.yuque.com/kenshin/simpread/apes3k ）

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## 使用 Assistive Touch 插件替代快捷键加入稍后读

[Assistive Touch](https://simpread.ksria.cn/plugins/details/rsd4UIcDKY) 是简悦的一个插件，作用是为用户提供一个比浮动控制栏/快捷键更加便捷的快捷键操作面板，用户可以在设置一些常用的操作，效果如下：

![img](https://cdn.nlark.com/yuque/0/2022/png/353945/1667796716057-48e36703-df50-487a-8658-0aff759432ee.png)

当按下图设置后，就可以使用 Assistive Touch 替代快捷键 `d d` 来加入稍后读了。

![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221107_1667797265.png)

也可以参考 [为 Assistive Touch 设置好看的 Icon](https://github.com/Kenshin/simpread/discussions/1600#discussioncomment-3930672) 定制化你的 Assistive Touch。

## 阅读模式优化

当前配置包没有开启 **如果当前页面为适配站点，自动进入阅读模式** 的功能，如果需要开启请进入选项页 → 阅读模式，按下图所示开启。

![image-20221013091327937](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221013_1665623607.png)

当前配置库仅配置了少数派的白名单，例如进入 https://sspai.com/post/69972 后会自动进入阅读模式，白名单的位置在选项页 → 全局 → 白名单

![image-20221013091625016](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221013_1665623785.png)

简悦拥有多种自动进入阅读模式或聚焦模式的方案，包括：

- [使用白名单让任意页面实现【自动进入阅读模式】](https://github.com/Kenshin/simpread/discussions/1672)
- [当阅读模式并未符合你的期望时，如何进一步优化？](https://github.com/Kenshin/simpread/discussions/1554)
- [白名单](URL编辑器?id=白名单)、[黑名单](http://ksria.com/simpread/docs/#/URL编辑器?id=黑名单)、[排除列表](http://ksria.com/simpread/docs/#/URL编辑器?id=排除列表)、[延迟加载列表](http://ksria.com/simpread/docs/#/词法分析引擎?id=延迟加载) 的使用说明

更多关于阅读模式的技巧 [请看这里](https://github.com/Kenshin/simpread/discussions?discussions_q=label%3A%22read+mode%22)。