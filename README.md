
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







```

10352 git init
10353 git status
10354 git add .
10355 git commit -m “initial commit”
10356 git remote add origin https://github.com/xiaoweiruby/hello_app_101.git
10357 git push -u origin master
```
