# Base app Rails 5 + uJs
By ![HashDog Logo](https://hashdog.com/images/logo.svg)

## Getting started
Clone a boilerplate
```
git clone git@github.com:hashdog/rails-5-boilerplate.git [project name]
```
Run bundle in project folder
```
bundle
```
Setup db
```
bundle exec rake db:setup
```
Edit client name
```
nano +37 app/views/home/wellcome.html.erb
```
Add changes in your new local repository
```
git add app/views/home/wellcome.html.erb
```
Commit the changes
```
git commit -m "First commit"
```
Replace the origin with the client repository URL (example: `git remote set-url origin git@github.com:user/repo.git`)
```
git remote set-url origin [new client repository URL]
```
Push the changes
```
git push origin master
```
Create an app on heroku with two enviroments, staging and production
```
heroku create -a staging-[app name] --remote staging
heroku create -a [app name] --remote production
```
Create a branch for production
```
git checkout -b production
```
Deploy the starter app for staging and production
```
git push staging master
git push production production/master
```
# App Components
- Ruby 2.2.3
- Rails 5
- Postgres
- Devise
- Sass
- Bootstrap 3
