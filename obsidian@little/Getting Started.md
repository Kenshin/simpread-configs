<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221003_1664782925.png" /></p>

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

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

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

`Obsidian@simpread` 的名字是可以随便修改的，但修改后需要修改导入到 Obsidian 插件的对应内容，也就是要保证下图对应的名字是一致即可。

![image-20221001151914758](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221001_1664608754.png)

## 重置 Local REST API

因为配置包直接自带了 Local REST API，因此也自动分配了一个 Token，但每个使用此方式的用户对应的 Token 都是一样的，可以通过删除并重新安装 Local REST API 的方式生成一个新的 Token。

当重新生成了 Token 后请同时修改插件端的 Token，随便打开一个网址 e.g. https://sspai.com/post/69972 然后进入阅读模式 → 右下角触发器 → 动作 → 插件触发器 → 导入到 Obsidian 选项，按下图所示修改。

![image-20221001162223433](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221001_1664612543.png)
