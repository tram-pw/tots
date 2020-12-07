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
