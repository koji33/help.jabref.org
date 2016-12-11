---
title: JabRefとMac OS X
helpCategories: ["FAQ"]
---

# JabRefとMac OS X

## Q: ダウンロードして解凍した後，OS Xが「パッケージは壊れているため開けません．"ゴミ箱"に入れる必要があります．」と表示します．

A: Mac OS X Lionでは，システム環境設定の「セキュリティとプライバシー」でのGatekeeperのセキュリティ設定を「すべてのアプリケーションを許可」に一時的に変更することで，解決することができます．そうして，JabRefアプリを開くことができます．一度，アプリを開いた後，セキュリティ設定を元に戻しても，依然としてアプリを開くことができます．

## Q: JabRef 2.11には，正式なMac OS Xアプリケーションがありません．

A: JabRef 2.11は，Mac OS X用に動作するバージョンを提供することができませんでした．2.11版のjarを使用するか，それよりも新しい3.X版（これはMac OS Xを完全にサポートしています）を見てみてください．

## Q: JabRef 2.xからJabRef 3.xへ直接アップグレードすることは可能ですか．

A: 3.x用インストーラに変更があったため，JabRef 3.x版はすべてクリーンインストールをする必要があります．以前にインストールされた2.xアプリケーションは，「アプリケーション」フォルダから削除する必要があります．その後，最新のJabRef 3.x版をインストーラを使用して導入してください．JabRef 3.x版を使用するようになれば，JabRefのアップグレードにインストーラを使用できるようになります．

## Q: JabRefを導入しようとしていますが，「JabRef Installerは，開発元が未確認のため開けません．」と言われて進めません．

A: これを解除するには，代わりに，Ctrl+クリックを行って，「開く」を選択してください．すると，同じ警告が出ますが，解除する選択肢が与えられますので，インストールができるようになります．

## Q: JabRefを導入しようとしていますが，「JabRef Installer Error: Error downloading the Java(TM) Runtime Environment. Please check your internet connection and start setup again.」と言われて進めません．

A: この問題は，あなたがJava 8を導入しておらず，自動ダウンロードとインストールが，何らかの理由で失敗しているためです…．下記のアドレスから，手動でダウンロードできます：
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
