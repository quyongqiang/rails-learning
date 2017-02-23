在controller中定义initialize方法时，每次action访问都会执行一遍initialize，必须使用super，否则css无法加载。
```ruby
class CheckoutController < ApplicationController

  def initialize

    super
    puts "============ in initialize: "
    @total ||= 0

  end
  
end
```
