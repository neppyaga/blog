+++
title = "scalafmtで変数型指定部分のAlignを設定する"
date = "2021-01-24"
template = "post/post.html"
+++

# はじめに
NeovimからIntelliJに乗り換えた際、変数に対する型指定部分の整列処理に関して躓いたのでメモ。

<!-- more -->
やりたいことは以下のような整列処理。

{{ gist(url="https://gist.github.com/neppyaga/521f278078a1a74a180d0e7d2cbd728c") }}

のようなコードを、以下のように整列させたい。
{{ gist(url="https://gist.github.com/neppyaga/93adacc3d316e6df9a56ab73d52343f1") }}

Neovim時代は`vim-easy-align`というvimプラグインを用いていた。

[junegunn/vim-easy-align: A Vim alignment plugin](https://github.com/junegunn/vim-easy-align)

ただideaVImで上記プラグインは対応していないらしい。ので、IntelliJでどうやって整列処理を行うか色々と試した。

# 解決策
IntelliJによるCaretを用いた整列を行うプラグイン等を試したが、マウスを使ってCaretの対象箇所を指定する方法があまり馴染まなかったので、一旦scalafmtによって解決することにした。

※マウスを使わずとも簡単に本記事例のようなCaretを指定できる方法をご存知の方がいましたらコメントいただけると幸いです。

`.scalafmt.conf`の設定は以下、
```conf
version = 2.5.0

align.tokens = [
  { code = ":", owner = ".*" }
]
```

# おわりに
自分が調べた限りだと公式ドキュメントに例が載っていなく、解決まで時間がかかってしまいましたが過去のPRからテストコードを探し出すことができました。めでたし。

以下、参考リンクです。

- [Configuration · Scalafmt](https://scalameta.org/scalafmt/docs/configuration.html#alignment)

- [Align types of class arguments · Issue #174 · scalameta/scalafmt](https://github.com/scalameta/scalafmt/issues/174)

- [Add support to align by tokens that have no space before them by olafurpg · Pull Request #441 · scalameta/scalafmt](https://github.com/scalameta/scalafmt/pull/441)
