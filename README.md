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
### 1 Filtering a List Using a Computed Property
```
remove(todo){
  this.todoItems = this.todoItems.filter(item=>item!=todo);
}
```


### 2 Sorting a List Using a Computed Property
```
sortedUsers(){
  if(!this.sortingKey){
    return this.users;
  }
  return this.users.concat().sort((userA,userB)=>{
    if(userA[this.sortingKey]>userB[this.sortingKey]){
      return 1;
    }
    if(userA[this.sortingKey]<userB[this.sortingKey]){
      return -1;
    }
    return 0;
  });
  }
}
```
### Currency
```
filters:{
  currency(value,options){
    if(!value){
      return '';
    }
    return formatMoney(value,options);
  }
}
```
