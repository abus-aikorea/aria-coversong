# Aria-CoverSong

🌍 [한국어](README.kor.md) ∙ [English](README.eng.md) ∙ [中文简体](README.zh.md) ∙ [中文繁體](README.tw.md) ∙ [日本語](README.jpn.md)

[![GitHub License](https://img.shields.io/github/license/abus-aikorea/aria-coversong)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases)

The best gradio web-ui for creating cover song that uses mdx-net and rvc. Easy one click installation. Fully portable.


### 実行画面

https://github.com/abus-aikorea/aria-coversong/assets/161691694/721b08b3-b1d8-48a2-ab59-f05b697ef95f



## はじめに
* Aria-CoverSongで**AI Cover**を簡単に作成してください。
*IUの「キューピット」、キム・グァンソクが歌う「見たい」、「二等兵の手紙」トランプ版を作ってみてください。
* UVR5が提供する**ボーカルリムーバー**と**RVC**エンジンを搭載しています。
* Aria-CoverSongは**ワンクリック**で簡単にインストールでき、Gradio Web-UIを提供します。
*最高レベルの**AI音声変調**技術を体験してください。


##主な機能

* `AI Cover`タブ
  - YouTubeダウンローダ、ボーカル分離、音声変調を統合環境で提供
  - ピッチ、ゲイン、リバーブ、ルーム、ダンピングなどのオーディオエフェクトをサポート

<p align="center">
  <img style="width: 90%; height: 90%" src="images/main_page.jpn.png?raw=true" alt=""/>
</p>  

* `Demixing`タブ
  - ボーカル分離、Reverb/Echo除去
  - MDX-Net、Demucsモデルのサポート
  - オーディオフォーマット（wav、flac、mp3）選択可能



## 主な特長
* YouTube動画（mp4、webm）をダウンロードし、オーディオファイル（mp3、wav、flac）として保存できます。
*ボーカルリムーバーを提供します。 **MDX-Net** と **Demucs** を利用します。
*音声変調機能を提供します。 **RVC v2** を利用します。
* AI Voice は **Discord AI Hub** からダウンロードするか、必要に応じて **制作依頼(abus.aikorea@gmail.com)** 可能です。
* **ワンクリックインストール**。一度インストールすると、追加料金なしで**永続**として使用できます。 （※Freeバージョンは利用時間**30分制限**あり）
* **Web-UI**を提供します。 Google Chromeブラウザをお勧めします。


## 商品説明文
* OS : Windows 10/11 (64bits) **※ Linux, Mac OSには対応しておりません。**
* CPU: Intelプロセッサ 2GHz以上(または同等の互換プロセッサ)
* RAM: 4GB 以上
* HDD: 10GB以上の空き容量(インストール時)
* GPU: :CUDA 11.8に対応するNVIDIAグラフィックカードを推奨。VRAM 4GB以上。
* インターネット接続環境必須(インストール時)


## インストールと実行

### step 1. パッケージの準備
* A.有料バージョン
    + USBに含まれる圧縮ファイル（**aria-coversong-x.zip**）をコンピュータの適切な場所に解凍する
    +またはすでに解凍されているフォルダ（**aria-coversong-x**）をコンピュータの適切な場所にコピーする

* B. 無料版
  + [![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/aria-coversong)](https://github.com/abus-aikorea/aria-coversong/releases) から最新リリース (**Source code (zip)**) ダウンロード後に解凍
  +または、git cloneでソースコードをダウンロードする

```bash
git clone https://github.com/abus-aikorea/aria-coversong.git
```

### step 2. プログラムのインストールと実行
1. `configure.bat`の実行
   - WindowsにffmpegとCUDA（NVIDIA GPUを使用している場合）をインストールします。
   - 最初の1回だけ実行するだけです。
2. `start.bat`の実行
   - Aria-CoverSongを起動します。 Web-UIが自動的に起動します。
   - 最初の実行時には、Aria-CoverSongのインストール作業を先に進めます。
   - Aria-CoverSongインストールはインターネット接続を必要とし、システムによってはインストールに1時間以上かかることがあります。
   - インストール中は絶対にWindowsコマンドウィンドウを終了しないでください。
   - インストール中に問題が発生した場合は、installer_filesフォルダを削除してstart.batを再実行してください。
#### Browserが自動的に実行されない場合
- Windows-Commnadウィンドウを終了し、start.batを再実行するか、
- ブラウザを直接実行し、Windowsコマンドウィンドウに表示されているアドレス（例：**http://127.0.0.1:7892**）をアドレスウィンドウに入力します。




### step 3. プログラムの削除
* `uninstall.bat`実行：
  - installer_filesフォルダを削除します。
  - Windowsにインストールしたffmepg、CUDAパッケージを削除します（選択した場合）

* Aria-CoverSongは**ポータブル**インストールがデフォルトです。プログラムの削除は、インストールフォルダを削除するだけで十分です。

## 注意事項
Windows Defenderが誤ってバッチファイルをトロイの木馬として認識している場合、これはしばしば「False Positive」と呼ばれます。この問題を解決するには、次の手順を実行できます。

1. ファイル例外処理：Windows Defenderでは、特定のファイルまたはプロセスがセキュリティチェックをスキップするように設定できます。これを行うには、以下の手順に従ってください

   * 「スタート」ボタンをクリックして「設定」に進みます。
   * [アップデートとセキュリティ]をクリックしてください。
   * 「Windowsセキュリティ」を選択し、「ウイルスと脅威の保護」に進みます。
   * [ウイルスと脅威の保護設定の管理]をクリックしてください。
   * 「ウイルスと脅威の保護設定」で「例外を追加」を選択してください。
   * 「ファイルまたはフォルダ」を選択し、問題のバッチファイルを見つけて例外として追加します。
2.  Windows Defender をしばらく無効にする: この方法は一時的な解決策になります。ただし、この方法を使用すると、コンピュータが他の脅威にさらされる可能性があるため、注意が必要です。

3. ワクチンソフトウェアに問題を提起: ファイルがトロイの木馬ではないという確信があれば、マイクロソフトに False Positive として情報を提供できます。マイクロソフトはこれを確認した後、必要な措置を講じます。


## 製品お問い合わせ
* メール: <abus.aikorea@gmail.com>
* ホームページ(韓国語): <https://slashpage.com/abus>
* 네이버 스마트스토어(韓国語): <https://smartstore.naver.com/abus/category/ALL?cp=1>
* Coupang(韓国語): <https://www.coupang.com/vp/products/7875503674>
* Amazon(英語): <https://www.amazon.com/dp/B0CTQQDPXT>
* Amazon(日本語): <https://www.amazon.co.jp/dp/B0CTHT2JH3>


## YouTube
* 商品説明: <https://youtu.be/heEN4UIQLjc>
* 自動字幕・翻訳: <https://youtu.be/uQ14hoEiI4c?si=Io9K_vIDYyeu9Z8_>
* ホームカラオケ: <https://youtube.com/playlist?list=PLwx5dnMDVC9bd6y3wXs-bOas2cXIi-GAq&si=B4S8HJr8gmeAw8hw>


## Credits
* RVC-Project: <https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI>
* UVR5: <https://github.com/Anjok07/ultimatevocalremovergui>
* FacebookResearch Demucs: <https://github.com/facebookresearch/demucs>
* yt-dlp: <https://github.com/yt-dlp/yt-dlp>
* gradio: <https://github.com/gradio-app/gradio>


## 著作権
<img src="images/ABUS-logo.jpg" width="100" height="100"> by [ABUS](https://slashpage.com/abus)
