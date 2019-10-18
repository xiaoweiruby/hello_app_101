#一、新建一个程式
```
10340 mkdir rubyspace
10341 cd rubyspace
10342 rails new hello_app
10343 ls
10344 cd hello_app
10346 bundle install
10348 atom .
10349 rails server

```


#二、增加一个功能


app/controllers/application_controller.rb

```

class ApplicationController < ActionController::Base
 def hello
 render html: “hello, world!”
 end
end
```



config/routes.rb
```

Rails.application.routes.draw do
 root ‘application#hello’
end
```






#三、上传一段代码
```

10352 git init
10353 git status
10354 git add .
10355 git commit -m “initial commit”
10356 git remote add origin https://github.com/xiaoweiruby/hello_app_101.git
10357 git push -u origin master
```
升级ruby
https://www.jianshu.com/p/99b90985915b
此版本的Ruby在Heroku-18上不可用
https://stackoverflow.com/questions/56675227/this-version-of-ruby-is-not-available-on-heroku-18

#四、完成云端部署

```
heroku login
heroku create hello_app_101
heroku create
git push heroku master
heroku open
```
