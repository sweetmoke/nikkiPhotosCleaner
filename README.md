<a href="README.en.md">Read the English</a>

## 本 Fork 与原项目的区别

本仓库是基于 [RanAxro/nikki_albums](https://github.com/RanAxro/nikki_albums) 的非官方改进版。原项目及其主要功能由 RanAxro 开发，本仓库在保留原有功能和整体结构的基础上进行了以下调整：

- **界面视觉优化**：依据仓库中的 `DESIGN-airbnb.md` 调整配色、字体层级、圆角、菜单、提示框与滚动条等视觉细节，并移除了窗口外围不协调的黑色边框；不改变原有功能和主要布局。
- **按日期批量选择照片**：每个日期分组标题前增加复选框，可以一次选中或取消选中该日期下的全部照片；手动选中部分照片时显示半选状态，也可以同时选择多个日期，再使用原有的删除、移出、导出等批量操作。
- **照片悬浮按钮提示**：鼠标悬浮在照片右侧的操作图标上时，会显示“标签”或“添加到参数管理器”，便于识别按钮功能；其中参数管理器按钮用于保存照片解析出的相机参数或分享码。
- **新增“导出高清并清理”功能**：在高清相册中选中照片后，可以将 High Quality 文件导出到用户指定的本地文件夹。文件复制并校验成功后，源 High Quality 文件会移入软件回收站。
- **可选择清理同图的其他版本**：执行上述操作前会弹出确认窗口，可选择是否一并清理 Low Quality、Screenshot、Magazine Photos、Clock-In Photo 和 Collage Photo 版本；默认选中 Low Quality 与 Screenshot。所选文件同样移入软件回收站，不是直接永久删除。
- **更安全的导出处理**：目标目录存在同名文件时自动生成不冲突的文件名；某张照片导出或校验失败时，不会清理该照片的源文件及其他版本。
- **限制 IndexNow 工作流**：向原作者网站 `nikki.ranaxro.com` 提交更新通知的工作流只允许在原仓库 `RanAxro/nikki_albums` 中执行，避免本 Fork 误通知原作者的网站。

> “导出高清并清理”会移动照片文件。首次使用时建议先选择少量照片测试，并确认导出结果无误。

---

以下为原项目的 README 内容：

<div align="center">
  <img src="assets/logo/nikkialbums.webp" alt="Nikki Albums", width="100", height="100">
  <br/>
  <h1>暖暖相册</h1>
</div>

<p>
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS-blue?style=flat-square" />
  
  <a href="https://github.com/RanAxro/nikki_albums/releases/latest">
    <img alt="Release" src="https://img.shields.io/github/v/release/RanAxro/nikki_albums?style=flat-square&color=brightgreen" />
  </a>

  <a href="https://nikki.ranaxro.com">
    <img alt="website" src="https://img.shields.io/badge/website-visit-yellow?style=flat-square&logo=home-automation&logoColor=white" />
  </a>

  <a href="https://github.com/ChanIok/SpinningMomo/blob/main/LICENSE">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-orange?style=flat-square" />
  </a>
</p>

<p>
  <img src="https://file-nikki.ranaxro.com/images/web/p1.zh.webp" width="48%" />
  <img src="https://file-nikki.ranaxro.com/images/web/p2.zh.webp" width="48%" />
</p>
<p>
  <img src="https://file-nikki.ranaxro.com/images/web/p3.zh.webp" width="48%" />
  <img src="https://file-nikki.ranaxro.com/images/web/p4.zh.webp" width="48%" />
</p>



<h2>🌟 游戏相册管理的得力助手</h2>

暖暖相册（Nikki Albums）是一款管理`无限暖暖`各种相册和分享码的软件。

🚀 **当前版本**：3.010

- **GitHub下载**：[点击这里](https://github.com/RanAxro/nikki_albums)  
- **官网下载**：[点击这里](https://nikki.ranaxro.com)  

💡 **交流群/bug反馈群**：1062670402  
加入我们，与其他玩家交流使用心得，反馈使用过程中遇到的问题，共同推动软件的优化与升级。

***

# 🎯 功能亮点

- **自动识别游戏**：无需手动设置，软件自动识别你的游戏，快速定位相册内容。
- **多账号分开管理**：轻松管理多个游戏账号的相册，互不干扰，让每个账号的相册都井井有条。
- **支持管理全部相册**：19个相册与3个游戏资源相册。
- **支持批量操作**：批量处理相册中的照片，一键备份、还原、转移、删除、复制、移动，大幅提升管理效率。
- **智能处理重复照片**：在转移或删除照片时，自动处理游戏保存的重复照片，避免冗余，保持相册的整洁有序。
- **简单创作**：支持简单裁剪图片与调色。
- **导出到网络**：允许在同一网络下传输图片。
- **转换实况(安卓/苹果格式)或gif动图**：支持将"动态影集"或"外部视频"相册的视频转换为实况或gif动图。
- **相册解码功能**：查看拍摄地点与相机参数，轻松复现拍过的美照。
- **参数管理器**：支持相机参数、搭配码以及家园码的管理与解析


***

# 更新内容

## v3.010
- 功能
  1. 参数管理器增加搜索功能，支持搜索名称、标签、衣服名、套装名、灯光、滤镜
  2. 粘贴或填写时自动剔除分享码里的文字或无关符号
  3. 增加生成搭配码二维码功能
  4. 搭配码历史记录顺序按时间倒序排序
  5. 支持自定义参数数据储存位置

- 性能与优化
  1. 优化ui

- bug修复
  1. 修复部分情况下，染色色盘显示错误的bug
  2. 修复织纹名称显示错误的bug
  3. 修复织纹绘制底色参数显示错误的bug


***

# 致谢

[暖暖共鸣录](https://gongeo.us/) > 提供无限暖暖套装服饰等图标  
[搬砖吧大喵](https://infinitymomo.com) > 家园码接口适配


***

<br/>
<div align="center" style="font-size: 20px">
  <a href="docs/declarations.zh.md">声明</a>
  &nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="docs/build.zh.md">构建</a>
</div>
<br/>
