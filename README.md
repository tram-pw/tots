# Team on the Snow !（tots/トッツ）

## 概要
### ■開発背景
&emsp;スポーツにおいて、コーチとプレイヤーの繋がりは非常に重要です。しかし時にその繋がりをオフラインで維持するのが難しいことがあります。  

例えば、様々な世代のプレイヤーを抱えるチームは大会が重なって他のチームに預けられるとか。ウイルス感染によって地元から出られないとか。  

そんな時にインターネットの力を使って繋がりを維持することで、その先にある「目標としていた大会で優勝することができた」「チームの力で勝つことができた」「コーチのおかげで自分の目指すべき方向が分かった」等、鳥肌が立つような感動体験が生まれると良いなと考えて開発をスタートしました。

### ■実現できること
&emsp;コーチ×プレイヤー、プレイヤー×プレイヤー、コーチ×コーチのコミュニケーション活性化

---
## 設計
### ■ターゲット

### ■シナリオ

### ■サイトマップ

### ■内部設計

---
## 機能
1. ベース機能（基本的にはスキー特化instagram）  
    ⇒共通
    - ゲストログイン機能
    - 新規登録/ログイン機能
    - フォロー機能
    - 動画/写真投稿
    - コメント/いいね機能
    - 保存(メモ)/グルーピング(独自タグ？)機能
    - 検索/ランキング機能
    - DM機能

2. コア機能（クローズド機能）  
    ⇒プレイヤー
    - チームへの参加申請
    - コーチへのレビュー依頼
    - コーチとのチャットQ&A
    - 日記/大会記録の投稿
    - 大会記録チャート
    - スケジュール/トレーニングメニューの共有
    
    ⇒コーチ
    - チームの作成/招待
    - プレイヤーへのレビュー回答
    - プレイヤーとのチャットQ&A
    - 日記/大会記録へのコメント
    - チームの大会記録チャート
    - スケジュール/トレーニングメニューの共有

3. おまけ機能（オープン機能。いわゆる独自のSNS機能）  
    ⇒共通
    - スキー場(大会)の地図表示（大会HPや速報サイトへのリンク？）
    - 優秀なチームランキング（戦績やいいね数？）
    - ブログ機能（noteやAmeba？とか表示するだけでも）

    ⇒プレイヤー
    - 大会単位のコメント/実況/参加表明
    - 一緒に練習したいボタン
    - コーチとのシンクロ率
    
    ⇒コーチ
    - 大会単位のアナウンス/参加表明
    - 教えたいボタン
    - プレイヤーとのシンクロ率

4. その他機能  
    ⇒共通
    - 翻訳（2か国語対応？日/英）
    - お問い合わせ(追加要望)機能

※コーチ/プレイヤーともに両方の属性を持つ可能性がある


---
## Setup

$ git clone git@github.com:tram-pw/tots.git <your project name>

project name -> <your project name> へ置換

$ heroku create

config/environments/production.rb
```
host = '<your heroku app>.herokuapp.com'
```

$ bundle install --without production

$ yarn install --check-files

$ rails db:migrate

$ rails db:seed

$ rails test

$ rails server

$ rm -rf .git/

$ git init

$ git add -A

$ git commit -m "first commit"

$ git remote add origin git@github.com:<username/projectname>.

$ git push -u origin master

$ git push heroku master

$ heroku run rails db:migrate

$ heroku run rails db:seed

$ heroku addons:create mailgun:starter

$ heroku addons:open mailgun

画面左側の「Sending」→「Domains」のリストにある「sandbox」で始まるサンドボックスドメインを選択します。画面右側の「Authorized Recipients」から受信メールアドレスを認証し、本番環境でのメール送信準備は完了です。

$ heroku rename <your project name>
