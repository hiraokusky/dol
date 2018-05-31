# dol

dockerを使ってインストールなしにいろんなツールを実行するためのスクリプトです。
現在、以下のツールに対応しています。

* sphinx
* gatling

# Usage

```
dol [tool] [command...]
```

# Requirements

* Docker
* Git for Windows (bashが実行できる環境)

# 準備

1. リポジトリをcloneします。
2. cloneしたディレクトリにパスを通します。
3. 各ツールのimageをつくるために、cloneしたディレクトリで "dol 各ツール名" を実行します。

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

# gatling

Gatlingは、WebAPIのパフォーマンステストを実行するツールです。

* https://gatling.io/

## シナリオを準備する

以下のディレクトリにシナリオを1つ置きます。
複数のシナリオには対応していません。

    ./user-files/simulations/computerdatabase/

以下を実行すると、シナリオの実行が開始されます。

```
dol gatling run
```

結果ファイルは以下のディレクトリに出力されます。
HTMLファイルになっており、ブラウザで結果を見ることができます。

    ./results/

結果ファイルを削除するには以下を実行します。

```
dos gatling clean
```
