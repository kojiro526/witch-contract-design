## あとがき

本書は技術書典5で頒布した『すべてのエクセルドキュメントを生まれる前に消し去りたい本　２０１８』[^techbook5]で紹介した方法を使って書かれている、サンプルドキュメントのようなものです。

本文はMarkdownで書かれた原稿をPandoc[^pandoc]を用いてdocxに変換しています。

図はスクリーンキャプチャを除いて、PlantUML[^plantuml]やnwdiag[^nwdiag]といったテキストベースの作図ツールを使っています。

本書のソースコードは以下のリポジトリにありますので、その気になれば自分でdocxファイルをビルドしていただくことも可能です。[^build]

[https://github.com/kojiro526/witch-contract-design](https://github.com/kojiro526/witch-contract-design)

Excelを使ったドキュメント作成に疲弊している世のSE・SIの皆さまが、軽量マークアップ言語によるドキュメント作成に手を出す際に、プレーンテキスト（Markdown）でだいたいどの程度の表現が可能なのか[^asciidoc]という参考にしていただけたら幸いです。

::: {custom-style="DateName"}
2019年8月12日

Kojiro
:::

[^techbook5]: [https://techbookfest.org/event/tbf05/circle/26870001](https://asciidoctor.org/)
[^pandoc]: [https://pandoc.org/](https://asciidoctor.org/)
[^plantuml]: [http://plantuml.com/ja/](http://plantuml.com/ja/)
[^nwdiag]: [http://blockdiag.com/ja/nwdiag/index.html](http://blockdiag.com/ja/nwdiag/index.html)
[^build]: 印刷版は、入稿のために背表紙にあたるページを手で付け加えたりしているため、ソースをビルドした状態とまったく同じにはなりません。
[^asciidoc]: もちろん、Markdownにこだわらず、Asciidoctor( [https://asciidoctor.org/](https://asciidoctor.org/) )などを使えばより豊かな表現でドキュメントを書くことができると思います。

