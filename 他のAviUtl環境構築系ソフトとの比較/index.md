---
title: 他のAviUtl環境構築系ソフトとの比較
description: AviUtl Installer Scriptと他のAviUtl環境構築系ソフトを比較します。
preview: https://aviutl-installer.github.io/img/Comparison-with-other-AviUtl-environment-construction-software-ja/ogp.png
---

# 他のAviUtl環境構築系ソフトとの比較
このページでは、AviUtl Installer Script と他のAviUtl環境構築系ソフトを比較しています。

## AviUtl Package Manager
AviUtl Installer Script と [AviUtl Package Manager](https://team-apm.github.io/apm/) (APM) を比較します。

### AviUtl Installer Script が優れている点
* **おすすめ構成が最新のものになっている**\
APMのおすすめには必須と言われるプラグインのうち、patch.aul と InputPipePlugin が含まれていない。また、APMのおすすめはインストールしようとしても L-SMASH Works が正常に導入されない (2025年1月現在) 。\
APMのおすすめに含まれている かんたんMP4出力 も更新が滞っており、バグ修正が行われていない。
* **初期設定の作業も自動で行われる**\
AviUtl Installer Script はAviUtl本体と必須プラグインを導入した後、環境設定や入力プラグイン優先度の設定など、初期設定も行っている。APMは設定作業は行わないため、利用者には初期設定に関する知識が必要。
* **操作がよりシンプル**\
AviUtl Installer Script はダブルクリックでファイルを実行するだけで作業が完了する。APMはインストールの際に開いたウィンドウでダウンロードするファイルのリンクをクリックするという手間がかかる。
* **Visual C++ 再頒布可能パッケージのインストールに対応している**\
AviUtl Installer Script は必須プラグインである patch.aul や有名なティム氏のスクリプトなどで必要となる、Visual C++ 再頒布可能パッケージのインストールに対応している。APMは対応していない。
* **古い/誤った情報を提供しない**\
APMはリポジトリの更新が遅く、パッケージの最新情報が提供されていないことも多い。導入されたパッケージのバージョンに関してもリポジトリの情報に準拠するため、正しくない情報が表示される。

### AviUtl Package Manager が優れている点
* **対応しているプラグインやスクリプトの種類が多い**\
AviUtl Package Manager は180以上のプラグインまたはスクリプトに対応しており、これらを簡単な操作でインストールできる。AviUtl Installer Script はいくつかのプラグインやスクリプトに対応予定だが、対応後もパッケージ数はAPMが圧倒的に多いだろう。
* **niconicoの親作品登録用のIDを取得できる**\
AviUtl Package Manager はniconicoの親作品登録用のIDを取得する機能がある。AviUtl Installer Script にはこの機能はない (多くの希望があれば実装するかもしれませんが、予定はありません) 。

### どちらを使うべき？ (ここまでの結論)
**AviUtlを導入する用途であれば AviUtl Installer Script を使用する方が良い**だろう。
* AviUtl Installer Script はAPMと比較して初心者により向いているため、AviUtlに関する知識が少ない内は AviUtl Installer Script を使用する方が良いと考えられる。
* AviUtlに関する知識をある程度持っている中級者以上のユーザーが、より多くのパッケージを楽にインストールしたいと思った場合にその欠点を理解しながら使うのであれば、おすすめなどを使用しない前提でAPMの機能の一部を利用すると快適かもしれない。
  * AviUtl Installer Script 1.1.2v2 (2025-01-22) 以降、インストールしたパッケージをAPMに認識させるための apm.json を配置するようになったため、パッケージの追加などを含めAPMを使用して AviUtl Installer Script で導入したAviUtl環境の管理を行うことが可能。

## AviUtl Extra Pack
AviUtl Installer Script と [AviUtl Extra Pack](https://www.videohelp.com/software/AviUtl) を比較します。

### AviUtl Installer Script が優れている点
* **おすすめ構成が最新のものになっている**\
AviUtl Extra Pack には**必須と言われるプラグインのうち、patch.aul と InputPipePlugin が含まれていない**。また、AviUtl Extra Pack がおすすめとしてインストールするプラグインには後継のプラグインが出ているような古いものも多い。
* **最新バージョンがインストールされる**\
AviUtl Extra Pack は**2019年後半から更新されておらず** (2025年1月現在) **、多くのプラグインがとても古いバージョンしかインストールされない**。必須とされるプラグインのうち AviUtl Extra Pack でインストールされる **L-SMASH Works や x264guiEx もかなり古いバージョンとなっている**。
* **ライセンスの問題がない**\
AviUtl Installer Script は全て配布サイトからダウンロードしているため、再頒布などによるライセンスの問題は発生しない。**AviUtl Extra Pack はライセンスが不明瞭であり、問題となる可能性もある**。
* **Visual C++ 再頒布可能パッケージのインストールに対応している**\
AviUtl Installer Script は必須プラグインである patch.aul や有名なティム氏のスクリプトなどで必要となる、Visual C++ 再頒布可能パッケージのインストールに対応している。AviUtl Extra Pack は対応していない。
* **導入後にAviUtl Package Managerが使用可能**\
インストールしたパッケージをAPMに認識させるための apm.json を配置するため、パッケージの追加などを含めAPMを使用して AviUtl Installer Script で導入したAviUtl環境の管理を行うことが可能。

### AviUtl Extra Pack が優れている点
* **インストールできるプラグイン・スクリプトが結構ある**\
AviUtl Extra Pack は50以上のプラグインまたはスクリプトに対応しており、これらを一括でインストールできる。AviUtl Installer Script はいくつかのプラグインやスクリプトに対応予定だが、対応後もパッケージ数は AviUtl Extra Pack の方が多いだろう。
* **英語/日本語の両方に対応している**\
AviUtl Installer Script は日本語にしか対応しておらず、インストール後の環境も日本語にしか対応していない。AviUtl Extra Pack は英語にも対応しており、英語対応の環境を構築することができる。

### どちらを使うべき？ (ここまでの結論)
**AviUtlを導入する用途であれば AviUtl Installer Script を使用する方が良い**だろう。
* AviUtl Extra Pack の古さやライセンスの不明瞭さ、不要な複雑さを考慮すれば、AviUtl Installer Script を使用する方が良いと考えられる。
* AviUtlに関する知識をある程度持っており、より多くのパッケージを楽にインストールしたいという中級者以上のユーザーであっても、AviUtl Extra Pack の古さやライセンスの不明瞭さを考慮すれば、APMを利用する方が良い。

## AviUtl-Installer-pwsh
AviUtl Installer Script と [AviUtl-Installer-pwsh](https://github.com/Per-Terra/AviUtl-Installer-pwsh/) を比較します。

### AviUtl Installer Script が優れている点
* **最新バージョンがインストールされる**\
AviUtl-Installer-pwsh では、**必須と言われるプラグインの patch.aul が** 謎さうなフォーク版 ではなく ePi版 、LuaJIT も 2.1.0 beta3 と**古いバージョンが指定されている**。また、AviUtl-Installer-pwsh は Aulsメモリ参照の1.00以降対応パッチ版 をインストールしようとするものの、リンク切れによりインストールできなくなっている。
* **現在も更新が続いている**\
AviUtl-Installer-pwsh は Aulsメモリ参照 のインストールができなくなっていることで、多くのファイルの配置やリネームにおける致命的な不具合を起こしており、**導入されたAviUtlをそのまま実行して使用することができない** (2025年3月現在) 。しかし、AviUtl-Installer-pwsh は**2022年前半から更新されておらず、2023年後半にはアーカイブされてしまっている**ため、これらの**問題が解消される可能性は低い**。
* **操作がよりシンプル**\
AviUtl Installer Script はダブルクリックでファイルを実行するだけで作業が完了する。AviUtl-Installer-pwsh はワンライナーをコピー&ペーストするだけで済むとはいえ、コマンドを入力する必要があり、またトラブルの少ないインストール場所を選択したりショートカットを作ったりはできない。
* **Visual C++ 再頒布可能パッケージのインストールに対応している**\
AviUtl Installer Script は必須プラグインである patch.aul や有名なティム氏のスクリプトなどで必要となる、Visual C++ 再頒布可能パッケージのインストールに対応している。AviUtl-Installer-pwsh は対応していない。
* **導入後にAviUtl Package Managerが使用可能**\
インストールしたパッケージをAPMに認識させるための apm.json を配置するため、パッケージの追加などを含めAPMを使用して AviUtl Installer Script で導入したAviUtl環境の管理を行うことが可能。

### AviUtl-Installer-pwsh が優れている点
* **rikkymodule&memory をインストールできる**\
AviUtl-Installer-pwsh では多くのプラグインやスクリプトが必要とする rikkymodule&memory を同時にインストールできる。AviUtl Installer Script も将来的に rikkymodule&memory のインストールに対応予定だが、2025年3月現在では AviUtl-Installer-pwsh がこの点では優れている。
* **手動でのダウンロードが不要である**\
AviUtl Installer Script は手動でダウンロードした後に実行する必要があるが、AviUtl-Installer-pwsh は実行するワンライナーによってコードが自動的にダウンロードされて読み込まれるため、手動でのダウンロードは不要となっている。そのため、常に最新版が使用されるほか、使用後のファイルが残らないという利点がある。

### どちらを使うべき？ (ここまでの結論)
**AviUtlを導入する用途であれば AviUtl Installer Script を使用する方が良い**だろう。
* AviUtl-Installer-pwsh の致命的な不具合や古さ、今後の更新が期待できないことを考慮すれば、AviUtl Installer Script を使用する方が良い。
* AviUtlに関する知識をある程度持っており、こういった致命的な不具合や古さに対応することができる中級者以上のユーザーであっても、わざわざ AviUtl-Installer-pwsh を選ぶだけのメリットがあまりなく、AviUtl Installer Script の使用後に手動またはAPMを用いて rikkymodule&memory をインストールする方が良いと考えられる。

## AviUtlAutoInstaller
AviUtl Installer Script と [AviUtlAutoInstaller](https://minfia.github.io/AviUtlAutoInstaller/) (AAI) を比較します。

### AviUtl Installer Script が優れている点
* **必須級のプラグインをまとめてインストールできる**\
AAIは最新のリポジトリにアップデートした後に**インストールを実行するとクラッシュしてしまい、インストールに失敗するため現状では利用不可能である** (2025年1月現在) 。\
~~また、インストールのチェックが入っているのはAviUtl本体と拡張編集Pluginのみであり、patch.aul、L-SMASH Works、InputPipePlugin、x264guiExはチェックを入れない限りインストールされない。~~
* **最新バージョンがインストールされる**\
~~AAIは[AAIのリポジトリ](https://github.com/minfia/AAI_Repo)に登録されたバージョンしかダウンロードしない。**AAIのリポジトリは2023年初頭から一切更新されておらず** (2025年1月現在) **、一部のプラグインはとても古いバージョンしかインストールされない**。~~
* **初期設定の作業も自動で行われる**\
AviUtl Installer Script はAviUtl本体と必須プラグインを導入した後、環境設定や入力プラグイン優先度の設定など、初期設定も行っている。~~AAIは設定作業は行わないため、利用者には初期設定に関する知識が必要。~~
* **操作がよりシンプル**\
AviUtl Installer Script はダブルクリックでファイルを実行するだけで作業が完了する。~~AAIはインストール項目一覧を開いて必要なものにチェックをつけてからインストールボタンを押すという手間がかかる。~~
* **導入後にAviUtl Package Managerが使用可能**\
インストールしたパッケージをAPMに認識させるための apm.json を配置するため、パッケージの追加などを含めAPMを使用して AviUtl Installer Script で導入したAviUtl環境の管理を行うことが可能。

### AviUtlAutoInstaller が優れている点
* ~~**有名なプラグイン・スクリプトは大体網羅している**\
APMほどではないものの、有名なプラグイン・スクリプトのだいたいに対応しており、これらを簡単な操作でインストールできる。AviUtl Installer Script はいくつかのプラグインやスクリプトに対応予定だが、対応後もパッケージ数はAAIの方が多いかもしれない。~~
* **ユーザーによる項目追加が可能**\
ユーザーによって追加できるユーザーリポジトリ機能があり、niconicoの親作品登録用のIDを含め、自分の追加したいものを追加 ~~してインストール、更新管理~~ することができる。

### どちらを使うべき？ (ここまでの結論)
そもそも**現状** (2025年1月現在) **AAIは使用できない**ため、AviUtl Installer Script とAAIのどちらかという選択肢であれば、**AviUtl Installer Script を使用するしかない**。
* ~~AviUtl Installer Script はAAIと比較してパッケージ数以外では大きく優れているため、AviUtl Installer Script を使用する方が良いと考えられる。~~
* AviUtlに関する知識をある程度持っており、より多くのパッケージを楽にインストールしたいという中級者以上のユーザーであっても、~~リポジトリが古すぎる上にパッケージ数もそこまで多くないので、~~ APMを利用する ~~方が良い~~ しかない。

## 結論
**AviUtlを導入する用途であれば AviUtl Installer Script を使用する方が良い**だろう。
* AviUtl Installer Script はAPMと比較して初心者により向いているため、AviUtlに関する知識が少ない内は AviUtl Installer Script を使用する方が良いと考えられる。
* AviUtlに関する知識をある程度持っている中級者以上のユーザーが、より多くのパッケージを楽にインストールしたいと思った場合にその欠点を理解しながら使うのであれば、おすすめなどを使用しない前提でAPMの機能の一部を利用すると快適かもしれない。
  * AviUtl Installer Script 1.1.2v2 (2025-01-22) 以降、インストールしたパッケージをAPMに認識させるための apm.json を配置するようになったため、パッケージの追加などを含めAPMを使用して AviUtl Installer Script で導入したAviUtl環境の管理を行うことが可能。
