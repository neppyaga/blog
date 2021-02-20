+++
title = "scalafmtで変数型指定部分のAlignを設定する"
date = "2021-01-24"
template = "post/post.html"
+++

# はじめに
NeovimからIntelliJに乗り換えた際、変数に対する型指定部分の整列処理に関して躓いたのでメモ。
<!-- more -->

やりたいことは以下のような整列処理。
```scala
case class User(
  id: User.Id,
  userName: UserName,
  email: EmailAddress
)
```
のようなコードを、以下のように整列させたい。
```scala
case class User(
  id:       User.Id,
  userName: UserName,
  email:    EmailAddress
)
```

Neovim時代は`vim-easy-align`というvimプラグインを用いていた。

[https://github.com/junegunn/vim-easy-align:embed:cite]

ただideaVImで上記プラグインは対応していないらしい。ので、IntelliJでどうやって整列処理を行うか色々と試した。

# 解決策
IntelliJによるCaretを用いた整列を行うプラグイン等を試したが、マウスを使ってCaretの対象箇所を指定する方法があまり馴染まなかったので、一旦scalafmtによって解決することにした。

※マウスを使わずとも簡単に本記事例のようなCaretを指定できる方法をご存知の方がいましたらコメントいただけると幸いです。

`.scalafmt.conf`の設定は以下、
```
version = 2.5.0

align.tokens = [
  { code = ":", owner = ".*" }
]
```

# おわりに
自分が調べた限りだと公式ドキュメントに例が載っていなく、解決まで時間がかかってしまいましたが過去のPRからテストコードを探し出すことができました。めでたし。

以下、参考リンクです。

[https://scalameta.org/scalafmt/docs/configuration.html#alignment:title]

[https://github.com/scalameta/scalafmt/issues/174:title]

[https://github.com/scalameta/scalafmt/pull/441:title]
