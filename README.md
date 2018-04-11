# ppvue2recipe
### Using Different Vue CLI Templates for Your Application
```
vue init webpack/simple appname
```

### Building a Simple Application with Vue
### Adding Interactivity to Your Web Application with Events

###  Constructing Your Own Vue Filters for Transforming Your Output
filters will automatically omit first param.
```
:value = "combined|reverse|wrap('(',')')"   //2 param
```


```
wrap:function(value,begin,end){   //3 param
  if(!value){return '';}
  return begin+value+end;
}
```
## 2. Computed Properties, Filters, and Conditionals
### 1 Filtering a List Using a Component Property
```
remove(todo){
  this.todoItems = this.todoItems.filter(item=>item!=todo);
}
```
