# [今日のシェルコマンド](/2014/08/04/shell-command-tr-split.html)

今日は必要に迫られてシェルのコマンドを調べて使った

# tr

単純な置換ができる

```
% cat file | tr '\n' ','
```

とすると改行を `,` に置換できる。ファイルの中身はパイプで渡してやる。なるほど。

# split

ファイルを行数単位、もしくはサイズ単位で分割ができる。

```
% split -l 1000 file
```

ちょっとした手作業もこうしたユーティリティを使えることが分かっているだけで作業がラクになったりするのでメモがてら。
