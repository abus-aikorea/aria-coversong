# Aria-CoverSong

🌍 [한국어](README.kor.md) ∙ [English](README.eng.md) ∙ [中文简体](README.zh.md) ∙ [中文繁體](README.tw.md) ∙ [日本語](README.jpn.md)

[![GitHub License](https://img.shields.io/github/license/abus-aikorea/aria-coversong)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases)

The best gradio web-ui for creating cover song that uses mdx-net and rvc. Easy one click installation. Fully portable.

### 运行界面

https://github.com/abus-aikorea/aria-coversong/assets/161691694/291ccd78-7812-4489-9df3-470b559de7ef

## 简介
* 使用 Aria-CoverSong 轻松创建 **AI 翻唱**。
* 制作 IU 的《Cupid》、金光石的《我想你》和《下士的信》的川普版本。
* 配备 UVR5 提供的**人声分离**和 **RVC** 引擎。
* Aria-CoverSong 可以**一键安装**，并提供 Gradio 网页界面。
* 体验最高水平的 **AI 声音调节**技术。

## 主要功能

* `AI Cover` 标签页
  - 提供 YouTube 下载器、人声分离和声音调节的集成环境
  - 支持音频效果，如音高、增益、混响、房间效果、阻尼等

<p align="center">
  <img style="width: 90%; height: 90%" src="images/main_page.eng.png?raw=true" alt=""/>
</p>  

* `Demixing` 标签页
  - 人声分离、混响/回音消除
  - 支持 MDX-Net、Demucs 模型
  - 可选音频格式（wav、flac、mp3）

## 主要特点
* 您可以下载 YouTube 视频（mp4、webm）并将其保存为音频文件（mp3、wav、flac）。
* 提供人声分离功能，使用 **MDX-Net** 和 **Demucs**。
* 提供声音调节功能，使用 **RVC v2**。
* AI 声音可以从 **Discord AI Hub** 下载，或根据需要**制作请求（abus.aikorea@gmail.com）**。
* **一键安装**。安装后，您可以**永久**使用，无需额外费用。（※ 免费版本使用时间限制为 **30 分钟**）
* 提供**网页界面**。推荐使用 Google Chrome 浏览器。

## 运行环境
* 操作系统：Windows 10/11（64位）**※ 不支持 Linux、Mac OS**
* CPU：Intel 处理器 2GHz 或更快（或兼容等效处理器）
* 内存：4GB 或以上
* 硬盘：安装时至少需要 10GB 可用空间
* 显卡：建议使用支持 CUDA 11.8 的 NVIDIA 显卡，VRAM 4GB 或以上
* 需要互联网连接（安装时）

## 安装和运行

### 步骤 1. 软件包准备
* A. 付费版本
    + 将 USB 中包含的压缩文件（**aria-coversong-x.zip**）解压到计算机适当位置。
    + 或者，将已解压的文件夹（**aria-coversong-x**）复制到计算机适当位置。

* B. 免费版本
  + 从 [![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases) 下载并解压最新版本（**Source code (zip)**）
  + 或者，使用 git clone 下载源代码

```bash
git clone https://github.com/abus-aikorea/aria-coversong.git
```

### 步骤 2. 安装和运行程序
1. 运行 `configure.bat`
   - 在 Windows 上安装 ffmpeg 和 CUDA（如果使用 NVIDIA 显卡）。
   - 只需首次运行一次。
2. 运行 `start.bat`
   - 启动 Aria-CoverSong。网页界面将自动运行。
   - 首次运行时，先安装 Aria-CoverSong。
   - Aria-CoverSong 安装需要互联网连接，根据系统配置可能需要超过一小时。
   - 安装过程中切勿关闭 Windows 命令窗口。
   - 如果安装过程中出现问题，请删除 installer_files 文件夹后重新运行 start.bat。

#### 浏览器未自动运行时
- 关闭 Windows 命令窗口并重新运行 start.bat。
- 直接运行浏览器并在地址栏输入 Windows 命令窗口中显示的地址（例如 **http://127.0.0.1:7892**）。

### 步骤 3. 卸载程序
* 运行 `uninstall.bat`：
  - 移除 installer_files 文件夹。
  - 移除在 Windows 上安装的 ffmpeg 和 CUDA 包（如果选择）

* Aria-CoverSong 采用**可携式**安装。要卸载程序，删除安装文件夹即可。

## 注意事项
当 Windows Defender 错误地将批处理文件识别为特洛伊木马时，这通常称为"误报"。要解决此问题，您可以按照以下步骤操作：

1. 文件例外处理：在 Windows Defender 中，您可以设置某些文件或进程跳过安全扫描。操作步骤如下：
   * 点击"开始"按钮，进入"设置"。
   * 点击"更新和安全"。
   * 选择"Windows 安全中心"并进入"病毒和威胁防护"。
   * 点击"管理病毒和威胁防护设置"。
   * 在"病毒和威胁防护设置"中选择"添加排除项"。
   * 选择"文件或文件夹"，找到相关批处理文件并将其添加为例外。

2. 临时禁用 Windows Defender：这可能是临时解决方案。但使用此方法时必须小心，因为可能会使您的计算机暴露于其他威胁之下。

3. 向防病毒软件报告问题：如果您确定该文件不是特洛伊木马，可以向 Microsoft 报告为误报。Microsoft 将审查并采取必要措施。

## 联系我们
* 电子邮件：<abus.aikorea@gmail.com>
* 主页（韩语）：<https://slashpage.com/abus>
* 韩国 Naver 智能商店：<https://smartstore.naver.com/abus/category/ALL?cp=1>
* Coupang（韩国）：<https://www.coupang.com/vp/products/7875503674>
* Amazon（美国）：<https://www.amazon.com/dp/B0CTQQDPXT>
* Amazon（日本）：<https://www.amazon.co.jp/dp/B0CTHT2JH3>

## YouTube
* 产品信息：<https://youtu.be/heEN4UIQLjc>
* 自动字幕∙翻译：<https://youtu.be/uQ14hoEiI4c?si=Io9K_vIDYyeu9Z8_>
* 家庭卡拉OK：<https://youtube.com/playlist?list=PLwx5dnMDVC9bVxfGo58U-R-w3fUHqwiD6&si=TZBh5AFjcr7_dyiI>

## 致谢
* RVC-Project：<https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI>
* UVR5：<https://github.com/Anjok07/ultimatevocalremovergui>
* FacebookResearch Demucs：<https://github.com/facebookresearch/demucs>
* yt-dlp：<https://github.com/yt-dlp/yt-dlp>
* gradio：<https://github.com/gradio-app/gradio>

## 版权
<img src="images/ABUS-logo.jpg" width="100" height="100"> by [ABUS](https://slashpage.com/abus)