<p align="center"><img src="https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665118121.png" /></p>

# 特点

1. 在阅读模式下加入稍后读，会自动生成本地快照和 PDF
1. 使用  `wkhtmltopdf`  作为 PDF 导出方案，此方案导出的 PDF 具有更多的定制化选项（细节请看附录）

# 适合用户

- 新用户，尤其是需要使用简悦剪藏网页的用户
- 喜欢使用 PDF 作为网页永久化保存的用户
- 不想折腾配置的用户

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

### 导入到 PDF 相关

- [修复标题因为特殊字符导致无法下载的问题](https://simpread.ksria.cn/plugins/details/tMGXrU1v0U)
- [自动化辅助增强](https://simpread.ksria.cn/plugins/details/DH9l5jblPH)
- [PDF 辅助增强插件](https://simpread.ksria.cn/plugins/details/Lly3mkuSPz)

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

## 设置 PDF 目录

如果不设置的话，会默认保存到 `output` 文件夹下，可以通过下面的方式将 `.pdf` 文件保存到本地的任意目录。

在同步助手 → 导出 → 增强导出

![image-20221007184641402](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665139601.png)

当生成 `.md` 文件后自动生成到 `Logseq@simpread` 文件夹。

```
{"extension":"pdf", "path":"/Users/xxxx/Ebook"}
```

如果是 Windows 系统的话，请使用下面的方案（留意有两个斜杠 `\\`）

```
{"extension":"pdf", "path":"C:\\Users\\***\\Ebook"}
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

此配置包内置了9个插件，导入成功后会有下图所示的提示。

![image-20220928104341346](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333021.png)

### 开启自动同步

使用此功能前，确保已经按照准备工作绑定了同步助手，选项页 → 共通 → 自动同步，开启下面的选项，并一定要选择 **通过简悦 · 同步助手覆盖本地配置文件**。

![image-20220928105621667](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664333781.png)

然后刷新当前页面，然后会在你的同步助手设置的同步文件夹下发现 `simprea_config.json` 文件，即说明导入成功。

![image-20220929184021771](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664448021.png)

## wkhtmltopdf

此配置包使用 [PDF 辅助增强插件](https://simpread.ksria.cn/plugins/details/Lly3mkuSPz) 内置的 wkhtmltopdf 作为 PDF 导出方案，所以还需要在你的本地下载并简单配置  `wkhtmltopdf` 。

### 下载

https://wkhtmltopdf.org/downloads.html 请根据自己的环境找到相应安装包。

### 验证

进入命令行，并执行 `wkhtmltopdf -V` 如果有类似输出的话，即说明安装成功。

![image](https://user-images.githubusercontent.com/81074/172299003-bcfaf031-b2bf-482e-9a9a-42e204c7a3fc.png)

### 设置目录

1. 如果是 Mac 用户的话，一般不需要设置 `wkhtmltopdf` 的目录
2. 如果你是 Windows 用户，尤其是 windows 11 的话，建议不要选择默认位置，请选择其它盘。

打开 https://sspai.com/post/71576 进入阅读模式 → 右下角 → 动作 → 插件触发器 → （打开）PDF 辅助增强选项，设置 `wkhtmltopdf` 目录，如下图

![image-20221007185959168](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20221007_1665140399.png)

上述完成后，此配置文件全部配置完毕。

## 测试

打开 https://sspai.com/post/71576 如果你的配置正确，应该会看到下图的界面并有一些现成的标注存在。

![image-20220928111105632](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220928_1664334665.png)

### 当加入稍后读后自动导出 PDF

https://user-images.githubusercontent.com/81074/194537377-0de19590-09ef-485d-aff0-9a44e23cd7fb.mp4

### 查看本地快照

打开稍后读，随便找一个已经存在的稍后读，如果有下面视频所示的标识则说明读取的本地文件。

https://user-images.githubusercontent.com/81074/192681150-f3986a9c-9983-4bae-b93b-768368b00bf5.mp4

# 附录

如果动手能力强的话，可以继续看看下面的一些技巧。

## wkhtmltopdf 相关

内置的 [PDF 辅助增强插件](https://simpread.ksria.cn/plugins/details/Lly3mkuSPz) 的配置中内置了 思源黑体，如果你本地也安装了思源黑体的话，导出的 PDF 字体就是思源黑体。

除此之外， **同步助手高级打印方案** 还提供了众多的定制化功能：

- [主题、字体样式、字体大小](https://github.com/Kenshin/simpread/discussions/3887#discussioncomment-2735661)
- [自定义字体](https://github.com/Kenshin/simpread/discussions/3887#discussioncomment-2735667)
- [自定义样式](https://github.com/Kenshin/simpread/discussions/3887#discussioncomment-2735664)
- [更细致的打印，如页边距、打印尺寸](https://github.com/Kenshin/simpread/discussions/3887#discussioncomment-2750058)
- 自带目录
- 完美解决因图片防盗链无法成功打印的问题

## 合并 output 和稍后读

如果你已经存在 output 并且也包含了一些稍后读，可以用任意文本编辑器分别打开你本地和解压缩后的的 `simpread_config.json` （假设你自己的叫 A，配置库的叫 B）

推荐使用 vs code 并安装 [ JSON Tools](https://marketplace.visualstudio.com/items?itemName=eriklynd.json-tools) 插件，然后对 `simpread_config.json` 格式化，找到 `unrdist`  并留意 `idx` （是一个自增长的 ID）

![image-20220929185850419](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449130.png)

把 B 中  `unrdist`  对应的内容全部复制到 A 并根据 `idx` 自增长进行排序，如下图所示

![image-20220929190305838](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449385.png)

然后把配置库中 `output` 文件夹对应的快照 id 也对应修改下。

![image-20220929190542971](https://cdn.jsdelivr.net/gh/23784148/upload-images@main/typora/20220929_1664449543.png)
