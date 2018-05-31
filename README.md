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

* docker
* bash

# 準備

1. リポジトリをcloneします。
2. cloneしたディレクトリにパスを通します。
3. 各ツールのimageをつくるために、cloneしたディレクトリで "dol 各ツール名" を実行します。

# 各ツールの使い方

* sphinx - https://github.com/hiraokusoy/dol/tree/master/sphinx
* gatling - https://github.com/hiraokusoy/dol/tree/master/gatling
