<p align="center"><img src="https://res.cloudinary.com/simpread/image/upload/v1733811527/config/7380e6938b1fddf1c5ee6901ada84ebf.png" /></p>

# 下载地址

[Github](https://github.com/Kenshin/simpread-configs/releases) 或 [百度云](https://pan.baidu.com/s/1SkFLJ21CKFL4lhWPhEg0iA?pwd=99mq) 请下载 `notion@sync.zip` 

# 特点

1. 内置 Notion 账户 及 Cloudinary 图床 [更多说明](https://www.yuque.com/kenshin/simpread/wpgqnh4eefgdx6o9)
2. 在阅读模式下使用快捷键 <kbd>f f</kbd> 触发图床插件，将图片转换为 Cloudinary 图床
3. 转换完图片后会自动加入稍后读，会自动生成本地快照
4. 在阅读模式下标注时，标注内容会自动同步到 Notion
5. 在阅读模式下标注时，标注内容会自动生成本地快照
6. 当稍后读、标注的元数据改变时，会自动导入 **带标注色的全文到 Notion** 以及 **导入标注到 Notion**

# 适合用户

- 新用户，尤其是需要使用简悦 + Notion 双链笔记配合的用户
- 不想折腾配置的用户
- 使用同步助手，非常适合重度使用简悦 + Notion 的用户

# 配置库文件说明

## 内置 Notion 账户

为了更直观的看到通过简悦导入到 Notion 后的效果，配置文件包含了简悦官方提供的 Notion 授权信息。

使用 `zaqr7s0g7@mozmail.com / sr123_654` 登录到 Notion 后可直接使用。

**注意**

1. 不要修改测试账户的密码，我会随时找回。😂
2. 不要删除任何其他用户导入的内容。
3. 测试账户只是让新用户更直观的看到通过简悦的导入效果，在使用时还是要更换为自己的账户。（附录有教程）

## 内置 Cloudinary 测试账户

下图来自 [图床插件](https://simpread.ksria.cn/plugins/details/VdMfVaXlni)

![image-20241210125205014](https://res.cloudinary.com/simpread/image/upload/v1733806328/config/c5572b45b64bddc118fbda220aa4ee02.png)

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

- [Assistive Touch - 类似 iOS 的快捷浮动工具栏](https://simpread.ksria.cn/plugins/details/rsd4UIcDKY)

- [阅读模式优化](https://simpread.ksria.cn/plugins/details/xZVbwW4C5A)

### 导入到 Notion 相关

- [导入到 Notion](https://simpread.ksria.cn/plugins/details/OpaogjT8KJ) （这是简悦官方推出的新插件用来取代扩展端导出 Notion 功能）

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)

- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)

- [导入到 Notion 辅助增强](https://simpread.ksria.cn/plugins/details/g60jwZEeqU)

### 本地快照相关

- [图床](https://simpread.ksria.cn/plugins/details/VdMfVaXlni)

- [稍后读辅助增强](https://simpread.ksria.cn/plugins/details/dtIMMLktg9)

- [插件管理器](https://simpread.ksria.cn/plugins/details/UEzvAXNSe5)

## 内置适配规则

内置两个跟 Notion 有关的适配规则。

![image-20241210130554922](https://res.cloudinary.com/simpread/image/upload/v1733807158/config/214e4c6a4d40cec5601e75e0a104067b.png)

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx) 并且 [绑定了同步助手](https://www.yuque.com/kenshin/simpread/pwpnsx)。
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

## 设置快照文件夹

也就是 `output` 文件夹，将下载的压缩包解压缩后放入到同步助手设置的同步盘文件夹。

![image-20241211081234913](https://res.cloudinary.com/simpread/image/upload/v1733875970/config/78a67696b7f932ae27704b9ec34bd647.png)

如果你已经存在 `output` 文件夹的话，可以先将 `output` 文件夹改名为 `output@origin` 或其它名字。

如果没有 `Output` 文件夹的话，在设置的同步文件夹下新建 `output` 即可，并在同步助手 → 导出 → 路径，添加 `output` 路径。

![image-20241211081304219](https://res.cloudinary.com/simpread/image/upload/v1733875987/config/cfdd1cfc12650595c13e81e5214829c5.png)

注意：`output` 文件夹不能改名，且必须要放到同步文件夹路径下面，也就是保证下面的结构，即 `simpread_config.json` 与 `output` 同级。

![image-20241211081344355](https://res.cloudinary.com/simpread/image/upload/v1733876026/config/a607996d781eb24fc825c9651be1779d.png)

## 导入配置文件

### 复制 UID

在选项页 → 账户 → 用户信息处复制你的 UID 到剪切板。（接下来的步骤会使用）

![image-20241210130625732](https://res.cloudinary.com/simpread/image/upload/v1733807191/config/d3c1348fda5dc868fa34ebb3fed1f897.png)

### 导入

建议使用一个新的浏览器或者在留存当前配置文件的前提下，重新安装简悦。安装完简悦后，通过选项页 → 共通 → 从本地导入配置文件到。

![image-20241210130651652](https://res.cloudinary.com/simpread/image/upload/v1733807215/config/679d26a93e177ac15ba66318eefc03f6.png)

### 恢复高级账户资格

导入并刷新后，进入账户 → 用户信息，修改为你自己的高级账户 UID（也就是在准备阶段让你复制的 UID）

![image-20241210130714215](https://res.cloudinary.com/simpread/image/upload/v1733807237/config/4422f1cf76d14facec9e2d040127a2d3.png)

保存后根据提示信息操作即可恢复你的高级账户资格。

![image-20241210130749465](https://res.cloudinary.com/simpread/image/upload/v1733807272/config/053e859c41d599641f0a58ec40c2f120.png)

### 导入插件

因为插件都比较大，因此并不包含在配置文件中，配置文件仅包含了插件的配置信息，因此导入新的配置文件后还需要导入插件，位置在：选项页 → 插件管理 → 从配置文件导入插件。

![image-20241210130847781](https://res.cloudinary.com/simpread/image/upload/v1733807330/config/7d76739550400d3b4910292af4eab05a.png)

此配置包内置了13个插件，导入成功后会有下图所示的提示。

![image-20241211081733680](https://res.cloudinary.com/simpread/image/upload/v1733876256/config/f59d6ab47bc5b39fdcb296aa4b5f3ea1.png)

### 开启自动同步

使用此功能前，确保已经按照准备工作绑定了同步助手，选项页 → 共通 → 自动同步，开启下面的选项，并一定要选择 **通过简悦 · 同步助手覆盖本地配置文件**。

![image-20241210192139952](https://res.cloudinary.com/simpread/image/upload/v1733829703/config/c71d7b9e1f5c3dfd1a00df48b15a55eb.png)

刷新当前页面，最后在你的同步助手设置的同步文件夹下发现 `simprea_config.json` 文件，即说明导入成功。

![image-20241211081807271](https://res.cloudinary.com/simpread/image/upload/v1733876291/config/499d9c7ec9a617f123cd4effb24abdd0.png)

上述完成后，此配置文件全部配置完毕。（下图是视频演示）

https://res.cloudinary.com/simpread/video/upload/v1733830646/config/2024-12-10_19-23-54_zbatxc.mp4

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20241210134402599](https://res.cloudinary.com/simpread/image/upload/v1733809447/config/5634b81a54f1d0d16e70e07f908ebeee.png)

### 在阅读模式下加入稍后读和标注

过程包括：

1. 使用快捷键 <kbd>f f</kbd> 触发
2. 触发图床插件，将图片转换为 Cloudinary 图床
3. 图片转换完毕后，加入稍后读
4. 生成本地快照
5. 标注
6. 标注完毕后修改稍后读元数据
7. 导入带标注色的全文到 Notion
8. 导入标注到 Notion

https://res.cloudinary.com/simpread/video/upload/v1733830771/config/2024-12-10_19-32-49_fvrn8m.mp4

### 查看本地快照

打开稍后读，随便找一个已经存在的稍后读，如果有下面视频所示的标识则说明读取的本地文件。

https://res.cloudinary.com/simpread/video/upload/v1733876369/config/192681150-f3986a9c-9983-4bae-b93b-768368b00bf5_opoeka.mp4

或者打开 https://sspai.com/post/71576 会在左下角看到下图所示的绿色标识。

![image-20241210194243503](https://res.cloudinary.com/simpread/image/upload/v1733830966/config/725beef7c092c0776e9d977dd37e0890.png)

# 如何使用

由于已使用配置好的方案（内置 Notion 账户和 Cloudinary 图床），因此无需进行任何额外设置。

进入任意 URL e.g. https://sspai.com/post/75567 使用快捷键 <kbd>f f</kbd> 触发导入到 Notion 的功能。

注意：

1. 这里的快捷键是 <kbd>f f</kbd> （图床的快捷键）而不是 <kbd>d d</kbd> 触发 <kbd>f f</kbd> 后产生的自动化细节可以看上面的 [阅读模式下加入稍后读和标注](#在阅读模式下加入稍后读和标注)
2. 这里并未加入 **添加/删除标注时自动导入标注到 Notion** 的功能，因为每次导入标注都会生成一个新的 Page。因此，自动化方案采用以下流程：

    > 加入稍后读 → 标注 → 添加稍后读元数据 → 触发 **导入全文到 Notion** 和 **导入标注到 Notion**。
    > 如果你希望每次标注都会自动导入到 Notion，请看附录里面的 [每标注一次即可同步一次到 Notion](#每标注一次即可同步一次到-notion)

# 注意事项

- 虽然内置了 Notion 账户和 Cloudinary 图床，但这些仅用于测试。正式使用前，请更换为自己的 Notion 和 Cloudinary 账户。更换方法详见附录。

- 使用此配置库方案**仅在阅读模式下使用**，在稍后读内置的阅读模式下无法使用。

- 使用此配置库方案**加入稍后读时只能使用快捷键** `d d` **或右键菜单的方式**，其它方式无法实现自动化。

​        ![image-20241210133234280](https://res.cloudinary.com/simpread/image/upload/v1733808757/config/2d3c1f05609f5950ed6088eabb2809f3.png)

- 建议不要删除已经存在的示例稍后读，当删除全部稍后读后，第一个稍后读会没有标号。（细节请看 https://www.yuque.com/kenshin/simpread/apes3k ）

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## 导入到 Notion（含 Notion 辅助增强和标注自动化） 教程

如果你想要对这套流程有更深入了解，可以看下这个教程 https://www.yuque.com/kenshin/simpread/zx3bcz

## 使用 Assistive Touch 插件替代快捷键加入稍后读

[Assistive Touch](https://simpread.ksria.cn/plugins/details/rsd4UIcDKY) 是简悦的一个插件，作用是为用户提供一个比浮动控制栏/快捷键更加便捷的快捷键操作面板，用户可以在设置一些常用的操作，效果如下：

![image-20241210133338217](https://res.cloudinary.com/simpread/image/upload/v1733808821/config/b5c5e5b6c1d9497cbc22e178e302f168.png)

当按下图设置后，就可以使用 Assistive Touch 替代快捷键 `d d` 来加入稍后读了。

![image-20241210133358570](https://res.cloudinary.com/simpread/image/upload/v1733808842/config/53b2c67defb7d32ad5b84f7cbedc17d6.png)

也可以参考 [为 Assistive Touch 设置好看的 Icon](https://github.com/Kenshin/simpread/discussions/1600#discussioncomment-3930672) 定制化你的 Assistive Touch。

## 更换自己的 Notion 账户

1. 退出测试 Notion 账户（如当前就是自己的 Notion 账户，可忽略此步骤）

2. 重新登录自己的 Notion 账户

3. 重启浏览器，随便打开一个页面 e.g. https://sspai.com/post/71576 并进入阅读模式 → 右下角 → 动作 → 插件触发器 → 导入到 Notion 选项

   ![image-20241209123622331](https://res.cloudinary.com/simpread/image/upload/v1733719649/config/473304f7b4e1617d6344c610d1ebac15.png)

4. **Duplicate** [此模板](https://simpread-nt-template.notion.site/29b7dc7dd5144f7598bdc6b0b1531a8f?v=10472d6ffb7b4b599f6b0af13ed44a26)，然后改名为 **来自简悦的稍后读**（或你喜欢的任意名称），也可以根据下图操作

   ![image-20241209125631968](https://res.cloudinary.com/simpread/image/upload/v1733720195/config/23524333f27ae68d17a0b2f29f97a848.png)

5. 选择授权 Notion 

   <video src="https://res.cloudinary.com/simpread/video/upload/v1733720318/config/2024-12-08_15-06-04_xx4wa0.mp4">

至此，完成全部设置。

## 更换自己的 Cloudinary 账户

请根据 [此教程](https://www.yuque.com/kenshin/simpread/wpgqnh4eefgdx6o9) 注册并获取到下图所示的 Cloud Name、API Key、API Secret，然后填入到下图所示位置即可。

![image-20241210132109563](https://res.cloudinary.com/simpread/image/upload/v1733808072/config/7f596f202d17d2b39e84360b2a29e25c.png)

## 合并 output 和稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20241210133451334](https://res.cloudinary.com/simpread/image/upload/v1733808902/config/825d27cf5c53ae891c6e5deff57824bb.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20241210131744938](https://res.cloudinary.com/simpread/image/upload/v1733807868/config/7c53f241536abe11c841dd2f425793ed.png)

## 每标注一次即可同步一次到 Notion

> 并不建议这么做，因为每次导入标注都会生成一个新的 Page。因此，自动化方案采用以下流程：
> 加入稍后读 → 标注 → 添加稍后读元数据 → 触发 导入全文到 Notion 和 导入标注到 Notion。

如果你希望每次标注都会自动导入到 Notion，请按下图修改自动化辅助增强插件

![image-20241210131652368](https://res.cloudinary.com/simpread/image/upload/v1733807815/config/2e3fdb66054efe55f36fc14144e9f7b2.png)

## 阅读模式优化

当前配置包没有开启 **如果当前页面为适配站点，自动进入阅读模式** 的功能，如果需要开启请进入选项页 → 阅读模式，按下图所示开启。

![image-20241210133700212](https://res.cloudinary.com/simpread/image/upload/v1733809023/config/e4795d7f21ed77262c6e6e22191b2394.png)

当前配置库仅配置了少数派的白名单，例如进入 https://sspai.com/post/69972 后会自动进入阅读模式，白名单的位置在选项页 → 全局 → 白名单

![image-20241210133730719](https://res.cloudinary.com/simpread/image/upload/v1733809053/config/40153c2d274a902b9a84df15ee04b820.png)

简悦拥有多种自动进入阅读模式或聚焦模式的方案，包括：

- [使用白名单让任意页面实现【自动进入阅读模式】](https://github.com/Kenshin/simpread/discussions/1672)
- [当阅读模式并未符合你的期望时，如何进一步优化？](https://github.com/Kenshin/simpread/discussions/1554)
- [白名单](URL编辑器?id=白名单)、[黑名单](http://ksria.com/simpread/docs/#/URL编辑器?id=黑名单)、[排除列表](http://ksria.com/simpread/docs/#/URL编辑器?id=排除列表)、[延迟加载列表](http://ksria.com/simpread/docs/#/词法分析引擎?id=延迟加载) 的使用说明

更多关于阅读模式的技巧 [请看这里](https://github.com/Kenshin/simpread/discussions?discussions_q=label%3A%22read+mode%22)。