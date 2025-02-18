---
en: true
title: What is AviUtl?
description: This page provides a brief description of AviUtl installed by the AviUtl Installer Script.
preview: https://aviutl-installer.github.io/img/en/What-is-AviUtl/ogp.png
---

## What is AviUtl?
### A lightweight and high-performance video editing software that can be used for free.
[AviUtl](http://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E3%81%95%E3%82%8C%E3%81%BE%E3%81%97%E3%81%9F%EF%BC%81-,%E2%98%85%20%E3%83%80%E3%82%A6%E3%83%B3%E3%83%AD%E3%83%BC%E3%83%89%20%E2%98%85,AviUtl,-aviutl110.zip%09version1.10) is software developed by a person named ＫＥＮくん, released in 1997, for cutting, filtering, and compressing [AVI files](https://en.wikipedia.org/wiki/Audio_Video_Interleave) (the standard video file format for Windows).\
In 2008, the creation of [拡張編集Plugin](http://spring-fragrance.mints.ne.jp/aviutl/#:~:text=%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%81%AF%E3%81%93%E3%81%A1%E3%82%89-,%E6%8B%A1%E5%BC%B5%E7%B7%A8%E9%9B%86Plugin,-%E5%8B%95%E7%94%BB%E3%80%81%E9%9D%99%E6%AD%A2%E7%94%BB) added many features, windows, objects, effects, and a timeline, making it a lightweight and high-performance video editing software that can be used for free.

Now, many plugins and scripts created by volunteers are actively being developed, adding functions, effects, animation effects, bug fixes, and optimizations. 

### What can you specifically do?
By adding scripts or skillfully using it according to what you want to do, you can create almost all the videos that are posted on YouTube.\
There are comments stating that such editing cannot be done with AviUtl, but it is almost certain that those people simply do not know how to do it.

### Complex Installation
Due to its history, AviUtl has become a state where several plugins other than the main AviUtl are practically essential, and it is also necessary to change settings to match modern usage scenarios, making the installation process complicated. Additionally, there is a lot of incorrect/old information online, making the installation very challenging.

Just the essential plugins include:

* 拡張編集Plugin version 0.92:\
Due to a critical bug in 0.93rc1, it is necessary to use 0.92.
* [patch.aul (謎さうな fork version)](https://github.com/nazonoSAUNA/patch.aul/releases/latest):\
A plugin that fixes bugs and speeds up AviUtl and 拡張編集Plugin. See [here (ja)](https://scrapbox.io/nazosauna/patch.aul) for details.
* [L-SMASH Works (Mr-Ojii version)](https://github.com/Mr-Ojii/L-SMASH-Works-Auto-Builds/releases/latest):\
An input plugin that supports a very large number of formats. With the advent of this plugin, most other input plugins have become unnecessary.
* [InputPipePlugin](https://github.com/amate/InputPipePlugin/releases/latest):\
A plugin that reduces errors by isolating the L-SMASH Works process in a 64-bit environment.\
99% of the cases where AviUtl crashes with a memory error during encoding can be resolved with this plugin.
* [x264guiEx](https://github.com/rigaya/x264guiEx/releases/latest) or similar output plugins:\
A plugin for outputting videos in the modern mainstream format of H.264/AVC + AAC in MP4.

There are five in total.\
Furthermore, there are various settings that should not be changed in the initial setup, as well as those that must be changed.

There are methods to install while watching newly updated and correct information in installation tutorial [videos (ja)](https://youtu.be/eFrIM0jP0qA) or [articles (ja)](https://scrapbox.io/aviutl/%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97), but [if you use the AviUtl Installer Script, you can complete the installation process with a double-click](../#how-to-use).
