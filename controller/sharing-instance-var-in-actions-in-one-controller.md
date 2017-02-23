http://stackoverflow.com/questions/9330486/same-instance-variable-for-all-actions-of-a-controller


```
def index
  set_up_instance_variable
end

def show
  set_up_instance_variable
end

private

def set_up_instance_variable
  @some_instance_variable = foo
end
```

