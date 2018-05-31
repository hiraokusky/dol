
# sphinx

Sphinxは、Markdown等で記述したテキストをHTML等にビルドするツールです。

* http://www.sphinx-doc.org/ja/stable/

標準で対応している機能は以下の通りです。

* commonmark==0.5.4
* recommonmark
* sphinx-autobuild
* sphinx_rtd_theme
* sphinxcontrib-mermaid

Makefileのあるディレクトリで実行します。

Sphinxの簡単なサンプルは、以下にあります。

* https://github.com/hiraokusoy/sphinx-samples

## ビルドしてHTMLファイルを作成する

```
dol sphinx html
```

## HTMLファイルを削除する

```
dol sphinx clean
```
