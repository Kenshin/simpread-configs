<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664946661.png" /></p>

# 下载地址

[Github](https://github.com/Kenshin/simpread-configs/releases) 或 [百度云](https://pan.baidu.com/s/1SkFLJ21CKFL4lhWPhEg0iA?pwd=99mq) 请下载 `notion@enhance.zip` 

# 特点

1. 导入到 Notion 时会将图片上传到 Notion （也就是开启了简悦的 Notion 图床功能），防止图片 404
2. 在阅读模式下加入稍后读，正文导入以 Markdown 的格式导入到 Notion
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
2. 不要删除任何其他用户导入的内容。
3. 测试账户只是让新用户更直观的看到通过简悦的导入效果，在使用时还是要更换为自己的账户。（附录有教程）

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

### 导入到 Notion 相关

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

# 注意事项

- 使用此配置库方案**仅在阅读模式下使用**，在稍后读内置的阅读模式下无法使用。

- 使用此配置库方案**加入稍后读时只能使用快捷键** `d d` **或右键菜单的方式**，其它方式无法实现自动化。

![img](https://cdn.nlark.com/yuque/0/2022/png/353945/1667796093600-99625a73-5cc8-4a9c-9118-526275035a12.png)

- 建议不要删除已经存在的示例稍后读，当删除全部稍后读后，第一个稍后读会没有标号。（细节请看 https://www.yuque.com/kenshin/simpread/apes3k ）

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## 使用 Assistive Touch 插件替代快捷键加入稍后读

[Assistive Touch](https://simpread.ksria.cn/plugins/details/rsd4UIcDKY) 是简悦的一个插件，作用是为用户提供一个比浮动控制栏/快捷键更加便捷的快捷键操作面板，用户可以在设置一些常用的操作，效果如下：

![img](https://cdn.nlark.com/yuque/0/2022/png/353945/1667796716057-48e36703-df50-487a-8658-0aff759432ee.png)

当按下图设置后，就可以使用 Assistive Touch 替代快捷键 `d d` 来加入稍后读了。

![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221107_1667797265.png)

也可以参考 [为 Assistive Touch 设置好看的 Icon](https://github.com/Kenshin/simpread/discussions/1600#discussioncomment-3930672) 定制化你的 Assistive Touch。

## 更换自己的 Notion 账户

1. 退出 Notion 账户

2. 重新登录自己的 Notion 账户

3. **Duplicate** [此模板](https://simpreadpublish.notion.site/e784eba882da452eb8f300e6cd6b195d)，然后改名为 **来自简悦的稍后读**，并对这个Page **加 Favorite** 操作。

   ![image-20221005114302175](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941382.png)

4. 简悦 → 选项页 → 服务 → 授权管理 → Notion → 取消授权 → 重新授权并找到到这个 Page

   ![image-20221005114328607](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941408.png)

5. 打开 https://www.notion.so/my-integrations 并添加一个 **新的 integration**

   ![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941457.png)

6. 然后按照下图设置

   ![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941489.png)

7. 其余内容默认值就可以， 确认无误后，选择 **Submit**，会得到下图

   ![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941525.png)



8.  复制上步位置的 Token 到剪切板
9. 邀请当前的 integration 到你（[第一步](https://github.com/Kenshin/simpread/discussions/3572#discussioncomment-2419547)）授权的 Page。

https://user-images.githubusercontent.com/81074/193977342-333fd5f2-2d38-4d34-9088-376c6ebec251.mp4

10. 打开第一步得到的 Page，例如 `https://www.notion.so/abcd****xyz?v=123***789` 这个 Page 对应的 ID 则是 **abcd\**\**xyz**

    ![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941718.png)

11. 随便进入一个页面 e.g. https://sspai.com/post/71576 并进入 **阅读模式 → 右下角触发器 → 动作 → 插件触发器**

    按照下图所示即可查看此插件的选项页。

    ![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221005_1664941750.png)

12. 刷新当前页面 e.g. https://sspai.com/post/71576 然后打开【导入到 Notion 辅助增强选项】，确认上述内容已填写。
13. 测试导入到 Notion，如果上述操作无误的话，会成功将当前页面导入到你的 Notion。

至此，完成全部设置。

## 合并稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20220929185850419](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449130.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20220929190305838](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449385.png)

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