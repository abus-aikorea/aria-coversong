# Aria-CoverSong

🌍 [한국어](README.kor.md) ∙ [English](README.eng.md) ∙ [中文简体](README.zh.md) ∙ [中文繁體](README.tw.md) ∙ [日本語](README.jpn.md)

[![GitHub License](https://img.shields.io/github/license/abus-aikorea/aria-coversong)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases)

The best gradio web-ui for creating cover song that uses mdx-net and rvc. Easy one click installation. Fully portable.

### 運行界面

https://github.com/abus-aikorea/aria-coversong/assets/161691694/291ccd78-7812-4489-9df3-470b559de7ef

## 簡介
* 使用 Aria-CoverSong 輕鬆創建 **AI 翻唱**。
* 製作 IU 的《Cupid》、金光石的《我想你》和《下士的信》的川普版本。
* 配備 UVR5 提供的**人聲分離**和 **RVC** 引擎。
* Aria-CoverSong 可以**一鍵安裝**，並提供 Gradio 網頁界面。
* 體驗最高水平的 **AI 聲音調節**技術。

## 主要功能

* `AI Cover` 標籤頁
  - 提供 YouTube 下載器、人聲分離和聲音調節的集成環境
  - 支援音頻效果，如音高、增益、混響、房間效果、阻尼等

<p align="center">
  <img style="width: 90%; height: 90%" src="images/main_page.eng.png?raw=true" alt=""/>
</p>  

* `Demixing` 標籤頁
  - 人聲分離、混響/回音消除
  - 支援 MDX-Net、Demucs 模型
  - 可選音頻格式（wav、flac、mp3）

## 主要特點
* 您可以下載 YouTube 視頻（mp4、webm）並將其保存為音頻文件（mp3、wav、flac）。
* 提供人聲分離功能，使用 **MDX-Net** 和 **Demucs**。
* 提供聲音調節功能，使用 **RVC v2**。
* AI 聲音可以從 **Discord AI Hub** 下載，或根據需要**製作請求（abus.aikorea@gmail.com）**。
* **一鍵安裝**。安裝後，您可以**永久**使用，無需額外費用。（※ 免費版本使用時間限制為 **30 分鐘**）
* 提供**網頁界面**。推薦使用 Google Chrome 瀏覽器。

## 運行環境
* 作業系統：Windows 10/11（64位）**※ 不支援 Linux、Mac OS**
* CPU：Intel 處理器 2GHz 或更快（或相容等效處理器）
* 內存：4GB 或以上
* 硬碟：安裝時至少需要 10GB 可用空間
* 顯卡：建議使用支援 CUDA 11.8 的 NVIDIA 顯卡，VRAM 4GB 或以上
* 需要網際網路連接（安裝時）

## 安裝和運行

### 步驟 1. 軟件包準備
* A. 付費版本
    + 將 USB 中包含的壓縮文件（**aria-coversong-x.zip**）解壓到電腦適當位置。
    + 或者，將已解壓的文件夾（**aria-coversong-x**）複製到電腦適當位置。

* B. 免費版本
  + 從 [![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases) 下載並解壓最新版本（**Source code (zip)**）
  + 或者，使用 git clone 下載源代碼

```bash
git clone https://github.com/abus-aikorea/aria-coversong.git
```

### 步驟 2. 安裝和運行程序
1. 運行 `configure.bat`
   - 在 Windows 上安裝 ffmpeg 和 CUDA（如果使用 NVIDIA 顯卡）。
   - 只需首次運行一次。
2. 運行 `start.bat`
   - 啟動 Aria-CoverSong。網頁界面將自動運行。
   - 首次運行時，先安裝 Aria-CoverSong。
   - Aria-CoverSong 安裝需要網際網路連接，根據系統配置可能需要超過一小時。
   - 安裝過程中切勿關閉 Windows 命令窗口。
   - 如果安裝過程中出現問題，請刪除 installer_files 文件夾後重新運行 start.bat。

#### 瀏覽器未自動運行時
- 關閉 Windows 命令窗口並重新運行 start.bat。
- 直接運行瀏覽器並在地址欄輸入 Windows 命令窗口中顯示的地址（例如 **http://127.0.0.1:7892**）。

### 步驟 3. 卸載程序
* 運行 `uninstall.bat`：
  - 移除 installer_files 文件夾。
  - 移除在 Windows 上安裝的 ffmpeg 和 CUDA 包（如果選擇）

* Aria-CoverSong 採用**可攜式**安裝。要卸載程序，刪除安裝文件夾即可。

## 注意事項
當 Windows Defender 錯誤地將批處理文件識別為特洛伊木馬時，這通常稱為"誤報"。要解決此問題，您可以按照以下步驟操作：

1. 文件例外處理：在 Windows Defender 中，您可以設置某些文件或進程跳過安全掃描。操作步驟如下：
   * 點擊"開始"按鈕，進入"設置"。
   * 點擊"更新和安全"。
   * 選擇"Windows 安全中心"並進入"病毒和威脅防護"。
   * 點擊"管理病毒和威脅防護設置"。
   * 在"病毒和威脅防護設置"中選擇"添加排除項"。
   * 選擇"文件或文件夾"，找到相關批處理文件並將其添加為例外。

2. 暫時禁用 Windows Defender：這可能是臨時解決方案。但使用此方法時必須小心，因為可能會使您的電腦暴露於其他威脅之下。

3. 向防病毒軟件報告問題：如果您確定該文件不是特洛伊木馬，可以向 Microsoft 報告為誤報。Microsoft 將審查並採取必要措施。

## 聯繫我們
* 電子郵件：<abus.aikorea@gmail.com>
* 主頁（韓語）：<https://slashpage.com/abus>
* 韓國 Naver 智能商店：<https://smartstore.naver.com/abus/category/ALL?cp=1>
* Coupang（韓國）：<https://www.coupang.com/vp/products/7875503674>
* Amazon（美國）：<https://www.amazon.com/dp/B0CTQQDPXT>
* Amazon（日本）：<https://www.amazon.co.jp/dp/B0CTHT2JH3>

## YouTube
* 產品資訊：<https://youtu.be/heEN4UIQLjc>
* 自動字幕∙翻譯：<https://youtu.be/uQ14hoEiI4c?si=Io9K_vIDYyeu9Z8_>
* 家庭卡拉OK：<https://youtube.com/playlist?list=PLwx5dnMDVC9bVxfGo58U-R-w3fUHqwiD6&si=TZBh5AFjcr7_dyiI>

## 致謝
* RVC-Project：<https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI>
* UVR5：<https://github.com/Anjok07/ultimatevocalremovergui>
* FacebookResearch Demucs：<https://github.com/facebookresearch/demucs>
* yt-dlp：<https://github.com/yt-dlp/yt-dlp>
* gradio：<https://github.com/gradio-app/gradio>

## 版權
<img src="images/ABUS-logo.jpg" width="100" height="100"> by [ABUS](https://slashpage.com/abus)