# 魔法少女契約管理システム設計書

## 本書について

本ドキュメントは、『すべてのExcelドキュメントを生まれる前に消し去りたい本』で紹介した方法を使って、Markdownでdocxファイルを生成する作例です。

- ドキュメントはMarkdownで書かれていますが、Pandocで変換することを前提としているため、処理系によっては正常に表示されません。
- 例えばVSCodeを利用しているなら、`Markdown Preview Enhanced`などの拡張昨日を使うことで、ローカルにインストールしたPandocでプレビューできるようになります。
- 一部の作図にはPlantUMLやnwdiagを使っています。

## docxのビルド方法

docxのビルドは以下のツールを使います。

[kojiro526/pandoc-pack](https://github.com/kojiro526/pandoc-pack)

上記のツールは、本書のような「部・章」構成でドキュメントを書くにあたって必要となる処理を行ったり、PlantUMLやnwdiagで書かれたソースから図を生成することも同時に行ってくれます。

てっとり速くビルドを試す場合はdockerイメージを利用します。（あらかじめdockerが使える状態である必用があります）

```
$ git clone https://github.com/kojiro526/witch-contract-design.git
$ cd witch-contract-design
$ dokcer pull kojiro526/pandoc-pack
$ docker run --rm -it -v $(pwd):/work kojiro526/pandoc-pack \
  build.sh -f -n -r ./template/reference-part-2.docx \
  -o ./tmp/witch-contract-design.docx \
  -p "--toc --toc-depth=3 --metadata=confidential=CONFIDENTIAL" ./src/
```

上記の結果、`./tmp/`ディレクトリ内にdocxファイルが生成されます。
