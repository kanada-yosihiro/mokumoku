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
### 選択した事業側の課題
サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？

### 提案内容
もくもく会をグループ(コミュニティ)で開催できるようにする
→現状、もくもく会への参加のハードルが高く、「男性だけが集まり自分だけ女性一人にならないかと心配している」などが考えられる。
  女性限定のグループや近い年代のグループを作り、参加しやすい環境を作る。
  
### 実装方針
- ヘッダーに「グループを作る」ボタンを追加する
- グループ一覧には「グループ名」、「グループ概要」、「参加者」、「開催予定のもくもく会」が表示される
- 同じグループに参加している人がもくもく会を開催したら、グループに参加している人全員に開催通知がいく
