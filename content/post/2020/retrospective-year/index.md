+++
title = "2020年振り返り"
date = "2020-12-31"
template = "post/post.html"
+++

# はじめに
年越しまで時間がないため殴り書きにはなりますが2020年の振り返りをしていこうと思います。

本記事は技術メインで振り返りをしていきます。

<!-- more -->

# 2019年末
2020年1月から内定先での内定者インターンが始まることが決まっていたため、インターンに向けた準備を進めていました。

内定先ではバックエンドにScala、フロントエンドにAngularを採用していました。

ScalaとAngularはほとんど触れたことがなかったため、ScalaとAngularを用いてシンプルなTodo管理を行うSPAを作成していました。

# 1~3月
4月の入社に向けて内定者インターンをしていた時期です。

いきなり実際のプロダクトに配属させてもらったのですが、業務未経験であったためにたくさんのことを学びました。

学んだことを大きく分けると以下のようになります。

- Webエンジニアとしての基礎的な知識
- Scalaの基礎文法
- HTML,CSSの基礎

## Webエンジニアとしての基礎的な知識
インターンが始まってすぐに自分の知識不足を実感しました。学んだ内容としては以下のような内容です。

- Git, Githubの使い方
- Vimの使い方
- スクラムの概要

以下、順に話していきます。

チーム開発経験がほとんどなかったため、Git, Githubに関して知らないことがたくさんあることを自覚しました。その際の学習で使用した教材は以下が良かったです。

[Lean Git Branching](https://learngitbranching.js.org/?locale=ja)


内定者インターンではVimを使用することになっていたためVimでのコーディングに慣れる練習をしました。最初は以下の教材で練習をしていました。

[Interactive Vim tutorial](https://www.openvim.com/)

配属チームではスクラム開発を採用しJiraでタスク管理を行っていました。スクラム開発は名前を聞いたことがある程度だったため概要を掴むためにインプットを行いました。

## Scalaの基礎文法
インターン中にScalaのコードを触っている際、なんとかコードを動かすことはできてもその背景にある知識が不足していました。


基礎知識を固めるため、2つの教材に取り組みました。

1つは「Tour of Scala」です。分からないこともありましたが6割くらいの理解で読み進めていたと思います。


[前書き | Scala Documentation](https://docs.scala-lang.org/ja/tour/tour-of-scala.html)

なんとか一周をして次の教材に進みました。

次はN予備校の「大規模Webアプリ Scala基礎コース」に取り組みました。

[N予備校 プログラミングコース](https://www.nnn.ed.nico/pages/programming/)

とても良質な教材で楽しく読み進めました。12章の「ケースクラスと同一性」等は今読んだとしても学びになるなと思います。


余談ですが、この時期に参加したScalathonというイベントがとても楽しかったです。


[Scalathon (Scala petit Hack-a-thon) - connpass](https://scalathon.connpass.com/)

初学者でも温かく迎えてくださり、Scalaの勉強に取り組むモチベーションがさらに上がるきっかけになりました。


## HTML,CSSの基礎
インターン中のタスクにある静的ページのデザインを丸々リニューアルするというタスクがあり、HTML, CSSにガッツリ取り組みました。

それまでは雰囲気でHTML,CSSを書いていたため、Progateで一通りのコースを学び基礎を固めました。

またCSSのクラス命名にはBEM記法が採用されていたためBEM記法についても学びました。

実践してレビューを頂きながら知識を身に付けることができたのでとても有り難かったなと思います。


# 4~6月
4月に入社をし、4月から5月の間オンラインで研修を行いました。

そして6月にプロダクトに配属され、いよいよ社会人としてのスタートを切った期間でした。

この時期に学んだことは以下のような内容です。

- Scala標準ライブラリ
- 状態管理・RxJS
- DDDのインプット

## Scala標準ライブラリ
入社後研修前半ではScala標準ライブラリに関する内容の基礎研修がありました。

具体的には社内のエンジニアの方々が作成された標準ライブラリに関する研修資料と実際のライブラリ実装コードを読みながら、自分の理解をテキストにまとめていきました。

これまでScalaの基礎文法については学習時間を多く取っていましたが、標準ライブラリに関しては理解度がそれほど深くなかったことを自覚しました。

参考資料として用意して頂いた「Scala実践入門」もとても分かりやすく、それまで曖昧に使っていたmap, flatMapやパターンマッチに関する動きを深く理解することができました。


[実践Scala入門：書籍案内｜技術評論社](https://gihyo.jp/book/2018/978-4-297-10141-1)

## 状態管理・RxJS
入社後研修後半では個人でTodo管理アプリケーションを作成する応用研修がありました。

フロントエンドにはAngularを使用したのですが、NGXSを用いて状態管理の概念に初挑戦しました。

NGXSの公式ドキュメントはとても分かりやすかったなと思います。

[Introduction - NGXS](https://www.ngxs.io/:embed:cite)


状態管理の概念と同時にRxJSに関しても学習を行いました。

初めてObservable型を見たときは正直なところチンプンカンプンでしたが、公式APIを参照しながらNGXS内で値をやり取りする処理を書くことで徐々に慣れていきました。

リアクティブプログラミングに関しては年末になった現在でもしっかりとした基礎のインプットができていないので、近いうちに深く理解する機会を作りたいなと思います。

## DDDのインプット
学生時代に少しだけ学んでいたDDDへの興味が再燃し、成瀬さんの「ドメイン駆動設計入門」を購入してDDDの学習をしました。

[ドメイン駆動設計入門  ボトムアップでわかる！ドメイン駆動設計の基本（成瀬 允宣）｜翔泳社の本](https://www.shoeisha.co.jp/book/detail/9784798150727)

値オブジェクトとエンティティの違い等が分かりやすく、サンプルコードもたくさんあったので気軽に読み進めることができました。

以降も楽しくDDDを学べているのはこの本で入門したおかげかなと思っています。

# 7~9月 
配属先の業務にも慣れてきて余裕ができたのか、様々なことをインプットしつつ初めてのLT発表にもチャレンジした時期でした。

その中でも大きなトピック挙げると以下の3つかなと思います。

- 関数型プログラミング（圏論）のインプット
- Scala RookiesでのLT発表
- 読書記録ブログ

## 関数型プログラミング（圏論）のインプット
しばしば名前だけ聞いていた「モナド」とはなんぞや？という疑問から始まり、関数型プログラミングや圏論に関することをインプットしていました。

Haskellや圏論の本を買って読んだり、個人開発でCatsライブラリを用いて色々処理を書いてみたりと細かく手を出していたと思います。

圏論に関しては、本の内容で分からない部分が多かったことからこのタイミングで一度挫折しているのですが、その後同期が社内勉強会で開催し始めた圏論勉強会を通して楽しく理解を深めています。

社内勉強会の内容は同期がブログにもまとめています。ありがたい。尊敬。

[圏論 カテゴリーの記事一覧 - ともちんの Tech ブログ](https://taretmch.hatenablog.com/archive/category/%E5%9C%8F%E8%AB%96:embed:cite)


## Scala RookiesでのLT発表
人生で初めてLT発表をしました。

内容は以下のブログにまとめています。

[scala.rookies #2に登壇してきた話. ネクストビートの20新卒エンジニアの久代です。普段は保育園の業務支援を行うKID… | by Taichi Kushiro | nextbeat-engineering | Medium](https://medium.com/nextbeat-engineering/scala-rookies-2%E3%81%AB%E7%99%BB%E5%A3%87%E3%81%97%E3%81%A6%E3%81%8D%E3%81%9F%E8%A9%B1-8572bcddabe4)

ファシリテーターにもチャレンジしたのですがとても緊張したのを覚えています。

その後オンラインイベント等に参加するとファシリテーターの方に注目して学びを得ることが習慣になりました。

## 読書記録ブログ
4~9月に読んだ本をまとめたブログを書きました。特に7~9月は色々な本を読んだなと思います。

[新卒エンジニアが入社半年でインプットした内容をまとめてみた. 20新卒エンジニアの久代です。… | by Taichi Kushiro | nextbeat-engineering | Medium](https://medium.com/nextbeat-engineering/%E6%96%B0%E5%8D%92%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%81%8C%E5%85%A5%E7%A4%BE%E5%8D%8A%E5%B9%B4%E3%81%A7%E3%82%A4%E3%83%B3%E3%83%97%E3%83%83%E3%83%88%E3%81%97%E3%81%9F%E5%86%85%E5%AE%B9%E3%82%92%E3%81%BE%E3%81%A8%E3%82%81%E3%81%A6%E3%81%BF%E3%81%9F-42ecc6a87fd3)


# 10~12月
この時期は以下の内容に力を入れていました。

- DDDのアウトプット
- 関数型プログラミングのアウトプット
- OOP・PofEAA・TDD・DDD周辺知識のインプット

## DDDのアウトプット
以下のスライドを読んだことをきっかけに、「自分もScalaでDDDのサンプルコードのようなものを書いてみよう」と思い立ちアウトプットをし始めました。

[scala-on-ddd - Speaker Deck](https://speakerdeck.com/crossroad0201/scala-on-ddd)

最終的に出来上がったものとしては、DDD開発の基盤として用いる自分用のライブラリ（librame）のようなものと

[neppyaga/librame: DDDを意識したWeb開発用ライブラリ。趣味を詰め込んでいる。](https://github.com/neppyaga/librame)

そのライブラリを用いたサンプルコードのような立ち位置である、簡単な認証機能を持つプロジェクトを作成しました。

[neppyaga/scala-ddd-auth-base: DDDを意識したユーザー認証基盤。librameライブラリのサンプルコード的な立ち位置](https://github.com/neppyaga/scala-ddd-auth-base)

プロジェクト内の採用技術はlibrameリポジトリのREADMEにまとめているのですが、その中でも特に学びが多かったのは[Eff](https://github.com/atnos-org/eff)と[Doobie](https://github.com/tpolecat/doobie)の2つのライブラリを導入した事かなと思います。

最初はCatsのEitherTで実装していたユースケース層の処理をEffで書き換えた事で、Effから受ける恩恵を実感しました。

Doobieライブラリに関しては必然的にCats Effectに関しても学ぶ必要があったため、Cats Effectのライブラリ（主にIOモナド）を読み込みました。

以上の2つのライブラリに関してはまだまだ理論や背景等の理解が足りていない部分が多いので、引き続き学習をしていきたいです。

## 関数型プログラミングのアウトプット
この頃から業務でもCatsライブラリに触れる機会が多くなり、「Catsライブラリを使うことに慣れてきたかな〜」と感じていたので「今度はCatsライブラリを作ってみよう。」と思い立ちました。

まだまだ道半ばでかつ最近は更新していないのですが、以下のリポジトリでゆるくアウトプットをしています。

[neppyaga/tabby: Catsライブラリをスクラッチから作りたい](https://github.com/neppyaga/tabby)

その途中で得た学びをZennに投稿してみました。

[ゼロから作るCatsライブラリ ~ implicit編 ~](https://zenn.dev/nepp_yaga/articles/cats-from-scratch-in-semigroup)

Githubリポジトリ・シリーズ化して投稿予定だったZennの記事ともに、途中で更新が止まっているので近いうちにまた力を入れて取り組み直したいです。やり抜くの大事。

## ソフトウェア設計に関する知識全般のインプット
最近はソフトウェア設計（この表現が正しいかも微妙）全般についての知識を、技術ブログ等でつまみ食いをしながらがむしゃらにインプットをしています。

キーワードとしては以下のような内容について興味を持っています。

- マイクロサービス
- ユビキタス言語
- ドメインモデル
- 契約による設計
- 概念モデリング
- PofEAA
- ICONIXプロセス
- 境界づけられたコンテキスト
- CQRS

最近はクリスマスにずっと欲しかったEvans本を書いました。上記のキーワードに関連する内容が多く登場するのでとても楽しく読ませていただいています。

「がむしゃらにインプットをしている」とは言いましたが、自分の興味のゆくままにインプットをしていると

- Martin Fowlerさん
- Bertrand Meyerさん
- Eric Evansさん

といったような偉大なる先人の方々の名前が登場する事が多いです。

そのため今後は上記の方々が残してくださった原典を中心に学習を続けていきたいなと考えています。

# おわりに
2020年の1年間を振り返ってみました。

1年間の振り返りをまとめるのは今回が初でしたが、実際に振り返ってみてとても良い区切りになったなと思います。

今後とも精進してドンドン成長していきたいです！

最後まで読んでいただきありがとうございました！
