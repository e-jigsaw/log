# [twlv というジョークライブラリをつくった](/2014/07/23/made-twlv.html)

https://github.com/jackdcrawford/five というライブラリがあって、ひたすら意味もなく 5 を複雑にするだけのライブラリでアホらしすぎて面白かった。

> This repo is absolutely fucking hilarious.
>
> Well done. Carry on.
>
> https://github.com/jackdcrawford/five/issues/79

とりあえず Japanese を追加するパッチを送ってみたりしたものの、それでは飽きたらなかったので自分でシュバッと作ることにした。

https://github.com/e-jigsaw/twlv.git

誰もしないとおもうけど、

```
% npm install twlv
```

するとすぐに試せるのでよければ。

`12` は自分にとって結構マジックナンバーなところがあるし、実際 `12` って時間が12進法だったり、十二神将とか、いろいろあるんじゃないかとおもって Wikipedia を調べてみたらあるわあるわという感じだったので勢いでばばっと作った。

めっちゃ意味のないテストを書いて、意味もなく Wercker で自動でテストが走るようにもした。そんだけです。
