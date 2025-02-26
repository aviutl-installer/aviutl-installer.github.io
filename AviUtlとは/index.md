---
title: AviUtlとは
description: AviUtl Installer Scriptがインストールする、AviUtlについて簡単に説明します。
preview: https://aviutl-installer.github.io/img/What-is-AviUtl-ja/ogp.png
---

## AviUtlとは
### 無料で使える軽量・高性能な動画編集ソフト
[AviUtl](http://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E3%81%95%E3%82%8C%E3%81%BE%E3%81%97%E3%81%9F%EF%BC%81-,%E2%98%85%20%E3%83%80%E3%82%A6%E3%83%B3%E3%83%AD%E3%83%BC%E3%83%89%20%E2%98%85,AviUtl,-aviutl110.zip%09version1.10)は ＫＥＮくん という方が開発し、1997年に公開した[AVIファイル](https://ja.wikipedia.org/wiki/Audio_Video_Interleave) (Windows標準の動画ファイルフォーマット) をカットしたり、フィルタをかけたり、圧縮したりするためのソフトです。\
2008年に[拡張編集Plugin](http://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%81%AF%E3%81%93%E3%81%A1%E3%82%89-,%E6%8B%A1%E5%BC%B5%E7%B7%A8%E9%9B%86Plugin,-%E5%8B%95%E7%94%BB%E3%80%81%E9%9D%99%E6%AD%A2%E7%94%BB)というものが作られたことで、タイムラインを始めとして多くの機能やウィンドウ、オブジェクト、エフェクトなどが追加され、無料で使える軽量・高性能な動画編集ソフトになりました。

今では有志によるプラグインやスクリプトが多数製作され、機能やエフェクト・アニメーション効果などの追加、バグ修正、軽量化などが活発に行われています。

### 具体的に何ができるの？
自分のやりたいことに合わせてスクリプトを追加したりうまいこと使いこなせば、YouTubeに投稿されているような動画はほぼ全て作成することができます。\
AviUtlではこういった編集はできない、といった書き込みもありますが、ほぼ確実にその人がやり方を知らないだけだったりします。

### 導入が大変
AviUtlはその歴史から、AviUtl本体以外にもいくつかのプラグインが事実上必須と言える状態になっており、また現代の利用シーンに合わせて設定も変更する必要があるなど、導入作業が複雑な上にネット上には誤った/古い情報も多く、導入がとても大変になっています。

必須とされるプラグインだけでも
* 拡張編集Plugin version 0.92:\
0.93rc1は致命的な不具合があるため0.92を使用する必要がある。
* [patch.aul (謎さうなフォーク版)](https://github.com/nazonoSAUNA/patch.aul/releases/latest):\
AviUtlと拡張編集Pluginのバグ修正と高速化を行うプラグイン。詳細は[こちら](https://scrapbox.io/nazosauna/patch.aul)。
* [L-SMASH Works (Mr-Ojii版)](https://github.com/Mr-Ojii/L-SMASH-Works-Auto-Builds/releases/latest) (lwinput):\
非常に多くの形式に対応した入力プラグイン。このプラグインの登場で大半の入力プラグインが不要になった。
* [InputPipePlugin](https://github.com/amate/InputPipePlugin/releases/latest):\
64bit環境でL-SMASH Worksのプロセスを分離してエラーを減らすプラグイン。\
「AviUtlがエンコード時にメモリエラーで落ちる」現象の99%はこのプラグインで解決する。
* [x264guiEx](https://github.com/rigaya/x264guiEx/releases/latest)、あるいは類似した機能を持つ出力プラグイン:\
現代の主流であるH.264/AVC + AACのMP4で動画を出力するプラグイン。

の5つがあります。\
さらに、初期設定においても変更すべきでない設定から、逆に変更しなければならない設定まで様々です。

新しく正しい情報が反映された[導入解説動画](https://youtu.be/eFrIM0jP0qA)や[導入解説記事](https://scrapbox.io/aviutl/%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97)を見ながら導入する方法もありますが、[AviUtl Installer Scriptであればダブルクリックで導入作業を完了させることができます](../#使用方法)。

他のAviUtl環境構築系ソフトとの比較が見たい人へ→[他のAviUtl環境構築系ソフトとの比較](../他のAviUtl環境構築系ソフトとの比較/)
