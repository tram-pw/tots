## Setup

config/environments/production.rb
```
host = '<your heroku app>.herokuapp.com'
```

$ rm -rf .git/

$ git init

$ git add -A

$ git commit -m "first commit"

$ git remote add origin git@github.com:<username/projectname>.

$ git push -u origin master

$ heroku create

$ git push heroku master

$ heroku addons:create mailgun:starter

$ bundle install --without production

$ yarn install --check-files

$ rails db:migrate

$ rails db:seed

$ rails test

$ rails server
