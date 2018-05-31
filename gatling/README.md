
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
