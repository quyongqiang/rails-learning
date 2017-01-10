### new project
rails new blog
rails new simple_cms -d postgresql


### 启动服务器
rails server
rails s
rails s -p 4000 -b 0.0.0.0

### 查看路由表
rake routes

### 重新载入database.yml文件?
rake db:fixtures:load

### 开启thin server
rails s thin

### 在项目根目录下执行 rails c ,打开rails console
rails c

### load test data
rake db:fixtures:load

### in irb
irb > Post.first.method(:someotherrandommethod).source_location
irb > Post.method(:somerandommethod).source_location

### routes all
rake routes

###
rake db:migrate
bundle exec rake db:migrate

### 
rails g 回车，会看到帮助
rails g controller 回车 会看到g controller的具体帮助
rails g controller  controller1 view1 view2 view3 ...

### export schema
rake db:schema:dump

### clear log
rake log:clear

### inspect
object.inspect

### gem install
gem install --no-rdoc --no-ri rspec ci_reporter_rspec

### list output as yml format
```
# rails c
> Rails.application.config.assets.paths
> y _

```

### open gem dir
```
export BUNDLER_EDITOR=subl
bundle open jquery-rails
```
