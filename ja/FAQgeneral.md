---
title: 一般事項
helpCategories: ["FAQ"]
---

# 一般事項

## Q: 使っているプラグインが動作しなくなってしまいました．どうすればいいでしょうか．

A: 開発チームが，プラグインサポートを追随させることが難しくなったために，JabRef v3.0において，プラグインサポートが停止されました．しかしながら，プラグインをJabRefに統合させることは可能です．現状と議論については，[issue #152](https://github.com/JabRef/jabref/issues/152)をご覧ください．個々のプラグインについては，作者に連絡を取って，そのプラグインをJabRefコードに移植してもらうようにお願いしてみてください．

## Q: 仕事でJabRefを使っています．私のパブリケーションで，JabRefを引用すべきでしょうか．

A: JabRefを引用する義務はありませんが，引用していただけると，たいへん嬉しく思います．

{% raw %}
```
@Manual{JabRef_software,
  title = {JabRef},
  author = {{JabRef Development Team}},
  year = {2016},
  url = {http://www.jabref.org}
}
```
{% endraw %}

## Q: JabRefを使ったパブリケーションは，何かありますか．

A: 聞き及んだ範囲でのパブリケーションは，すべて<https://github.com/JabRef/jabref/wiki/JabRef-in-the-media>に収録してあります．

## Q: JabRefが起動しません．どうすればいいでしょうか．

A: これは，設定をリセットしなくてはならないせいかもしれません．`java -jar JabRef-X.Y.jar --prdef all -n`を実行してください(X.YはJabRefのバージョン)．Windowsでは，これがうまくいかない場合，`regedit`を実行して，`HKEY\_CURRENT\_USER\SOFTWARE\JavaSoft\Prefs\net\sf\jabref`というフォルダを削除してください．

## Q: JabRefは中国語をサポートしますか．

A: はい．**オプション → 設定 → 一般 → 既定エンコーディング** と進んで，UTF-8を選択してください．それから，**外観** で表フォントをsimsun (または他の中国語フォント)に設定してください．**一般** でUI言語を中国語にすることもできます．詳しい情報は，<http://yenlung.km.nccu.edu.tw/xms/read_attach.php?id=61> (あるいは<https://web.archive.org/web/20111027034912/http://yenlung.math.nccu.edu.tw/~yenlung/notes/latex_in_Windows.pdf>)にあります．

## Q: When I have an instance of Jabref running and double click another BibTeX file it is opened in a new JabRef instance. Is it possible to open it in a new tab in the first instance?

A: Yes. Go to **Options -&gt; Preferences -&gt; Advanced -&gt; “Remote operation”**.
Put a checkmark to “Listen for remote operation on port:”.
This option allows new instances of JabRef to detect the instance already running, and pass files to that instead of opening a new window.

## Q: I have a DOI. Is it possible to create an entry directly out of the DOI?

A: Yes. Go to Search and click on “Web Search” to enable the Web search.
A Web search box appears on the left side of JabRef.
The name of a web search is selected (e.g. “ACM Portal”).
Click on it and change it to “DOI to BibTeX”.
Enter the DOI in the field and press “Fetch”.
A search starts and the result is displayed in a new pop up window.
One entry should appear.
Just push “OK” to insert the entry into the database.

## Q: I have an ISBN. Is it possible to create an entry directly out of the ISBN?

A: Yes. Go to Search and click on “Web Search” to enable the Web search.
A Web search box appears on the left side of JabRef.
The name of a web search is selected (e.g. “ACM Portal”).
Click on it and change it to “ISBN to BibTeX”.
If a ISBN is not found, head to the [online service](http://manas.tungare.name/software/isbn-to-bibtex/) by Manas Tungare.

## Q: I miss a field translator, lastfollowedon, ... How can I add such fields?

A: To add this “translator“ to all entry types, you can use **Options-&gt;Set up general fields** and add a “translator” field under one of JabRef's general field tabs.
To add this "translator" to a specific entry type, edit the specific entry type(s) (**Options-&gt;Customize entry types**) and add a “translator“ field under required fields or optional fields, as you like.


## Q: How do I prevent JabRef from introducing line breaks in certain fields (such as “title”) when saving the .bib file?

A: Open **Options -&gt; Preferences**.
In the “File” panel, you will find an option called “Do not wrap the following fields when saving”.
This option contains a semicolon-separated list of field names.
Any field you add to this list will always be stored without introduction of line breaks.

## Q: I have a JabRef open. If I open a bibtex file from my web browser, a new JabRef is started. I want the file to be opened in the currently opened JabRef. Is this possible?

A: Yes. Go to **Options -&gt; Preferences -&gt; Advanced -&gt; “Remote operation”**.
Put a checkmark to “Listen for remote operation on port:”.
This option allows new instances of JabRef to detect the instance already running, and pass files to that instead of opening a new window.
Note: This is the default [since JabRef 3.0](https://github.com/JabRef/jabref/blob/master/CHANGELOG.md#30---2015-11-29).

## Q: Is it possible to append entries from a BibTeX file, e.g. from my web browser, to the currently opened database?

A: Yes, you can use the parameter `--importToOpen bibfile`.

## Q: I want to link external files with paths relative to my .bib file, so I can easily move my database along with its files to another directory. Is this possible?

A: Yes. You need to override the default file directory for this specific database.
Go to **File -&gt; Database properties**. You can override the **Default file directory** setting.
There, you can either enter the path in **General file directory** (for it to be valid for all users of the file) or in **User-specific file directory** (for it to be valid for you only).
If you simply enter “.” (a dot, without the quotes), the file directory will be the same as the .bib file directory.
To place your files in a subdirectory called **subdir**, you can enter **“./subdir”** (without the quotes).
Files will automatically be linked with relative paths if the files are placed in the default file directory or in a directory below it.

## Q: I want to export my bibliography entries into a simple text file so that I can import them into a spreadsheet easily. Is this possible?

A: Yes. Use **File -&gt; Export**.
Under “Filter:”, choose “OpenOffice/LibreOffice CSV (\*.csv)”.

## Q: How can I add and remove keywords of multiple entries?

A: Select the entries.
Right click.
Choose “Manage keywords”.
Then you can manage keywords appearing in all selected entries or in any selected entry.
New keywords are added to all selected entries.

## Q: I want to have a bib-file-specific PDF directory.

A: Right click on the tab of the .bib file.
Choose “Database properties”.
Then at the field “General file directory” choose the directory specific for the database.
If you want to set a directory for you only (so that other users should use the default directory), use the field “User-specific file directory”.

## Q: When linking a file, I cannot set the correct type. How can I add new types?

A: Go to **Options -&gt; Manage external file types**.
Here you can add arbitrary types.

## Q: Is there a portable version of JabRef?

A: Store the file jabref.jar on the drive.
It can be opened directly on any computer offering a Java installation by double clicking the `jar` file.
In **Options-&gt;Preferences-&gt;General**, be sure to activate "Load and Save preferences from/to jabref.xml on start-up (memory stick mode)".

## Q: When an organization is provided as author, my BibTeX style doesn't recognize it. For instance, “European Commission” is converted to “Commission, E.”.

A: Use braces to tell BibTeX to keep your author field as is: `{European Commission}`.
In BibLaTeX, you can use `label = {EC}` to have `EC05` as label for a publication of the European Commission in the year 2005.

## Q: Is there a FAQ on BibTeX?

A: Yes, please look at “Bibliographies and citations” at the [UK List of TeX Frequently Asked Questions on the Web](http://www.tex.ac.uk/).
For German readers, there is the [dante e.V. FAQ](http://projekte.dante.de/DanteFAQ/LiteraturVerzeichnis).

## Q: Where is the RenameFile plugin? How to rename file automatically after importing entries?

A: JabRef does not support plugin anymore (version > 2.11). However the plugin features are progressively integrated.
Renaming of files is now part of the "Cleanup Entries" feature (brush button in the toolbar or CTRL+SHIFT+F7).
Then, you can rename attached files based on the BibTeX key.  You can change the format (pattern) under
**Options -&gt; Preferences -&gt; Import**, by altering the pattern under "Default PDF file link action".

## Q: I have a JabRef database and I would like to export a subset to BibTeX (or BibLaTeX) format. How to do this?

A: Your JabRef database is already a file in BibTeX (or BibLaTeX) format. Simply select the entries to be exported, and then
choose **File-&gt;Save Selected as...**. More details on [stackexchange.com](https://tex.stackexchange.com/questions/82554/jabref-can-it-export-a-subset-of-the-bibliography-in-bibtex-format).

## Q: I have a JabRef database and I would like to export the subset corresponding to my LaTeX file. How to do this?

A: Upon compilation, LaTeX generates a file with the extension ".aux". This files contains the keys of the cited references (among other things). Using this AUX file, JabRef can extract the relevant entries. Choose the menu **Tools-&gt;New subdatabase based on AUX file**. Then select the reference database (among the opened ones), and specify the AUX file.


## Q: When I modify my database, I would like that JabRef performs entry cleaning automatically. How to do this?

A: In **File-&gt;Database properties**, you will find a section named "Save actions". After enabling this feature, you can choose which actions should be performed for each field upon saving. That should help you keep your database tidy.

## Q: Search on Google scholar does not work anymore. What is going on?

A: Google scholar is blocking "automated" crawls which generate too much traffic in a short time. JabRef already uses a two-step approach (with the prefetched list before crawling the actual BibTeX data) to circumvent this.
However, after too much crawls JabRef --- or more correct: your IP address --- is being blocked.
To unblock your IP, do a Google scholar search in your browser. You will be asked to show that you are not a robot.

Thus, the Google Scholar fetcher is not the best way to obtain lots of entries at the same time. If you are using Mozilla Firefox, the JabRef Plugin "JabFox" might be an alternative to download the BibTeX data directly from the browser. You can find the PlugIn here: https://addons.mozilla.org/en-US/firefox/addon/jabfox/?src=external-jabrefSite
