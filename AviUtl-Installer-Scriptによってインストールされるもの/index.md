---
title: AviUtl Installer Scriptによってインストールされるもの
description: AviUtl Installer Scriptがインストールする、AviUtlとそのプラグインやスクリプトなどの一覧です。
preview: https://aviutl-installer.github.io/img/List-of-items-installed-by-AviUtl-Installer-Script-ja/ogp.png
---

# AISによってインストールされるもの

いつの間にか増えてきてしまったので一覧です。

## インストールされるもの
AviUtl Installer Script [1.1.18 (2025-02-26)](https://github.com/menndouyukkuri/aviutl-installer-script/releases/tag/v1.1.18) の aviutl-installer.cmd によってインストールされるものの一覧です。\
バージョンや日付の記載がないものはインストール時の最新版がインストールされます。

### AviUtl本体
- **[AviUtl version 1.10](https://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E2%98%85%20%E3%83%80%E3%82%A6%E3%83%B3%E3%83%AD%E3%83%BC%E3%83%89%20%E2%98%85-,AviUtl,-aviutl110.zip%09version1.10%092019/10/3)**\
最大4GBまでしかメモリを使用できないという従来の制限を**突破した**最新バージョン (と言っても2019年だが) 。

### AviUtlプラグイン
- **[拡張編集Plugin version 0.92](http://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%81%AF%E3%81%93%E3%81%A1%E3%82%89-,%E6%8B%A1%E5%BC%B5%E7%B7%A8%E9%9B%86Plugin,-%E5%8B%95%E7%94%BB%E3%80%81%E9%9D%99%E6%AD%A2%E7%94%BB)**\
タイムラインを始めとして多くの機能を追加する必須のプラグイン。0.93rc1は致命的な不具合があるため0.92にしている。
- **[patch.aul (謎さうなフォーク版)](https://github.com/nazonoSAUNA/patch.aul/releases/latest)**\
AviUtlと拡張編集Pluginのバグ修正と高速化を行う必須級のプラグイン。詳細は[こちら](https://scrapbox.io/nazosauna/patch.aul)。
- **[L-SMASH Works (Mr-Ojii版)](https://github.com/Mr-Ojii/L-SMASH-Works-Auto-Builds/releases/latest)** (lwinput)\
非常に多くの形式に対応した必須級の入力プラグイン。このプラグインの登場で大半の入力プラグインが不要になった。
- **[InputPipePlugin](https://github.com/amate/InputPipePlugin/releases/latest)**\
64bit環境でL-SMASH Worksのプロセスを分離してエラーを減らす必須級のプラグイン。\
「AviUtlがエンコード時にメモリエラーで落ちる」現象の99%はこのプラグインで解決する。
- **[x264guiEx](https://github.com/rigaya/x264guiEx/releases/latest)**\
現代の主流であるH.264/AVC + AACのMP4で動画を出力する必須級のプラグイン。
- **[NVEnc](https://github.com/rigaya/NVEnc/releases/latest)** / **[QSVEnc](https://github.com/rigaya/QSVEnc/releases/latest)** / **[VCEEnc](https://github.com/rigaya/VCEEnc/releases/latest)** のうち、**その環境で使用できる中で画質が良いもの1つ**\
ソフトウェアエンコード (x264guiExもこれ) より高速で軽いが若干品質が落ちる、ハードウェアエンコードで動画を出力するプラグイン。\
(どれも使えない環境ではどれもインストールされません)
- **[MFVideoReader](https://github.com/amate/MFVideoReader/releases/latest)**\
デコードに[Media Foundation](https://ja.wikipedia.org/wiki/Media_Foundation)を使用する入力プラグイン。[メディア プレーヤー](https://apps.microsoft.com/detail/9wzdncrfj3pt?hl=ja-jp&gl=JP)で再生可能な動画・音声ファイルを読み込むことができるが、不具合もあるため最終手段。

### Susieプラグイン
Susieという画像ビューアのプラグインです。不完全ながら拡張編集Pluginで画像を読み込むために使用できます。
- **[WebP Susie Plug-in Version 1.1](http://toro.d.dooo.jp/slplugin.html#iftwebp)**\
アルファ付き.webpを読み込めるようにするSusieプラグイン。
- **[ifheif](https://github.com/Mr-Ojii/ifheif/releases/latest)**\
HEIF ( .heif , .heic ) / AVIF ( .avif ) を読み込めるようにするSusieプラグイン。

### スクリプト
- **[AviUtlスクリプト一式 (さつきさん作) 20160828](https://bowlroll.net/file/3777)**\
さつきさんの作ったスクリプトの詰め合わせで、かなりの数の演出やオブジェクトが入っている。必須級のスクリプト。
- **[値で図形 v2.10](https://scrapbox.io/nanikani-shugo/Nagomiku%E8%87%AA%E4%BD%9C%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%97%E3%83%88)**\
標準の図形では縦横のサイズが違う図形を出すにはなぜか縦横比で調整する必要があるが、値で図形のカスタムオブジェクトを利用すれば縦横それぞれのサイズを指定できる。
- **[直線スクリプト (2021/03/07)](https://ux.getuploader.com/tikubonn_aviutl/download/1)**\
なぜか標準で存在しない、太さと長さを指定して直線を引けるカスタムオブジェクトを追加するスクリプト。中心点を変えたり先端を丸めたりすることもできる。

### その他
- **[LuaJIT](https://github.com/Per-Terra/LuaJIT-Auto-Builds/releases/latest)**\
拡張編集Pluginのスクリプトが使用するLuaを、トレーシング実行時コンパイルという技術を用いて高速化するもの。一部のエイリアスなどでも必要とされる。
- **[Visual C++ 再頒布可能パッケージ 2015-20xx (x86)](https://learn.microsoft.com/ja-jp/cpp/windows/latest-supported-vc-redist)**\
patch.aulなどのプラグインや一部のスクリプトで必要になる。2015-2022以降がインストールされる。
- **[Visual C++ 再頒布可能パッケージ 2008 (x86)](https://learn.microsoft.com/ja-jp/cpp/windows/latest-supported-vc-redist)**\
古いプラグインや一部のスクリプトで必要になる。それらを使わない人には不要なため選択式。
