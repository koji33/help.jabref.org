---
title: JabRefとWindows
helpCategories: ["FAQ"]
---

# JabRefとWindows

## Q: JabRefをMicrosoft Wordのバックエンドに使うには，どうすれば良いでしょうか．

A: Word内部の文献マネージャーで，直接文献を扱うことができます．簡単に説明すると，あなたの書誌情報をXML形式でエクスポートして，`%APPDATA%\Roaming\Microsoft\Bibliography`にあるSources.xmlを置き換えてください．詳しい説明については，[Using JabRef references in Word document](http://www.ademcan.net/?d=2012/01/30/15/23/05-using-jabref-references-in-word-documents)をご覧ください．

他の選択肢としては，[BibteX4Word](http://www.ee.ic.ac.uk/hp/staff/dmb/perl/index.html)を使う方法もあります．

もう一つの選択肢としては，JabRefへの移植が計画されている[Docear4Word](https://github.com/Docear/Docear4Word)を使うことです（[JabRef4Word](https://github.com/JabRef/JabRef4Word)をご覧ください）．

## Q: ホットキーWindows+JでJabRefを起動したり，フォーカスを当てたりするには，どうすれば良いでしょうか．

A: [koppor's autohotkey scripts](https://github.com/koppor/autohotkey-scripts)で提供されている[JabRef.ahk](https://github.com/koppor/autohotkey-scripts/blob/master/JabRef.ahk)と[AutoHotkey](http://www.autohotkey.com/)を使用してください．
