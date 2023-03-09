# README

## 環境構築
```
$ bundle install --without=production
$ bin/rails db:setup
$ yarn install
$ bin/webpack
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください
選択した事業側の課題
直近一年間で、2回以上もくもく会に参加してくれた人は利用者全体の1%のみ。もくもく会で気の合う仲間を見つけられなかったのではないか？

提案内容
課題から、１回目でミスマッチが起こっていると考えられる。
それを解決するために以下の提案を考えた。
例）そのイベントがどんなイベントかが分かりにくいので、イベントをジャンル分けして過去のイベントをイベント詳細画面で表示できるようにする。。
例）よりイベントのイメージをわかりやすくするため、イベントごとにアンケートをとり、イベント詳細画面で閲覧できるようにする。


実装方針
イベントを登録する際に、ジャンルが登録できるようにイベントテーブルに新しいカラムを追加し、登録ページで登録できるようにする。
イベント詳細画面に関連の過去のイベントを一覧で表示できるようにする。
イベントとアンケートを紐ずけるリレーションを組み、新たしくアンケート登録画面を実装する。
イベントに紐ずくアンケートの回答結果を過去のイベントの詳細画面に表示されるようにする。
