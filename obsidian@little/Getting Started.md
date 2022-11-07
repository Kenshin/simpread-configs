<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221003_1664782925.png" /></p>

# 下载地址

[Github](https://github.com/Kenshin/simpread-configs/releases) 或 [百度云](https://pan.baidu.com/s/1SkFLJ21CKFL4lhWPhEg0iA?pwd=99mq) 请下载 `obsidian@little.zip` 

# 特点

1. 在阅读模式下加入稍后读，会将正文导入以 Markdown 的格式导入到 Obsidian
2. 在阅读模式下标注时，标注内容会自动同步到 Obsidian
3. 不使用同步助手，非常适合轻量级使用简悦 + Obsidian 的用户

# 适合用户

- 新用户，尤其是需要使用简悦 + Obsidian 双链笔记配合的用户
- 不想折腾配置的用户

# 配置库文件说明

## 文件说明

- `Obsidian@simpread` → Obsidian 库文件，包含了跟简悦有关的一些插件
- `simpread_config.json` → 简悦配置文件，导入后即可使用
- `Getting Started.md` → 说明文档

## Obsidian 库文件说明

内置了跟简悦有关系的四个插件：

- Banners
- Dataview
- Local REST API

## 内置 Obsidian 模板

内置了一套 Obsidian 模板，如果对其它模板感兴趣的话，可以看看 [简悦的官方模板库](https://github.com/Kenshin/simpread/discussions/2153) 基本上满足大部分 Obsidian 用户需求。

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

# 教程

## 准备

1. 如果是老用户的话，请务必备份好你的之前的配置文件。（选项页 → 共通 → 导出配置文件到本地）
2. 如果是新用户的话，请先确保是 [升级为高级账户](https://www.yuque.com/kenshin/simpread/pwpnsx) 并且 [绑定了同步助手](https://www.yuque.com/kenshin/simpread/pwpnsx)。
3. 一般来说使用这套流程的用户都使用坚果云，所以先暂停坚果云的自动同步功能或退出坚果云。

## 设置 Obsidian 库文件夹

将解压缩的文件夹 `Obsidian@simpread` 放到你需要的任意目录，然后在 Obsidian 指定这个目录。

![image-20220928093550398](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664328950.png)

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

###  在阅读模式下标注

然后再开启 Obsidian 的前提下，增加新的标注，看看是否会自动同步到 Obsidian。

https://user-images.githubusercontent.com/81074/193401583-80a15ce4-4c98-40d1-909b-d1a7613b31e3.mov

# 注意事项

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

## 合并 Obsidian 配置

如果你已经存在了一些 Obsidian 插件，仅需要将 `Obsidian@simpread/.obsidian` 对应的文件夹复制到你自己的  `.obsidian` 然后打开 `.obsidian/community-plugins.json` 将下面的内容加入其中。

 ```
 "dataview",
 "obsidian-banners",
 "obsidian-local-rest-api"
 ```

## 合并 output 和稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20220929185850419](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449130.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20220929190305838](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449385.png)

## 修改文件夹的名字

`Obsidian@simpread ` 的名字是可以随便修改的，但修改后需要修改导入到 Obsidian 插件的对应内容，也就是要保证下图对应的名字是一致即可，只需要修改下面的两个地方：

- 导入到 Obsidian
- Obsidian SimpRead Sync

![img](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221107_1667795425.png)

## 设置多级目录

如果你需要在 Obsidian 上设置多级目录的话，，也就是要保证下图对应的名字是一致即可，只需要修改下面的两个地方：

- 导入到 Obsidian
- Obsidian SimpRead Sync

![img](https://cdn.nlark.com/yuque/0/2022/png/353945/1667795237494-7a2798de-102d-4229-af35-a85eb2752b79.png)

## 重置 Local REST API

因为配置包直接自带了 Local REST API，因此也自动分配了一个 Token，但每个使用此方式的用户对应的 Token 都是一样的，可以通过删除并重新安装 Local REST API 的方式生成一个新的 Token。

当重新生成了 Token 后请同时修改插件端的 Token，随便打开一个网址 e.g. https://sspai.com/post/69972 然后进入阅读模式 → 右下角触发器 → 动作 → 插件触发器 → 导入到 Obsidian 选项，按下图所示修改。

![image-20221001162223433](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221001_1664612543.png)

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