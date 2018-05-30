# dos

dos is docker on script.

# sphinx

build docker image.

```
dos sphinx build
```

run sphinx command.

```
dos sphinx make html
```

```
dos sphinx make clean
```

# gatling

build docker image.

```
dos gatling build
```

run gatling.

以下のディレクトリにシナリオを1つ置きます。
複数のシナリオには対応していません。

./user-files/simulations/computerdatabase/

実行.

```
dos gatling run
```

結果ファイルは以下のディレクトリに出力されます。

./results/

```
dos gatling clean
```
