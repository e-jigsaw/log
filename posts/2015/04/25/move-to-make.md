# [このブログを gulp から make に移行した](/2015/04/25/move-to-make.html)

gulp しんどいなってフェーズになってきたので、思い切って make ベースに移行してみた。しばらく gulp 外してどういう形態にするか悩んでいたが、make でタスクの管理をして、記事やアーカイブのところはベタにコード書いてしまうことにした。最後に PR を見てみると `+284 -381` でコード量の削減ができた。

ブログっぽい静的ページに必要なのは

* CSS や favicon などのコピー、コンパイル
* 記事の出力
* アーカイブページ
* RSS

あたりである。CLI で完結できるものは CLI で完結させて(CSS のコピーとか、Stylus のコンパイル)足りないものはコードに落とす方針でいった。ファイルの扱いなどをどうしようか迷ったが、gulp で `src` に使われている glob を使うことで解決した。変に Stream とか絡まなくなった分、スッキリした印象。

変更内容に興味あるひとは PR 見てみてくださ〜い。[#59](https://github.com/jgsme/dev/pull/59)

ついでに LiveScript にも移行してたりする。
