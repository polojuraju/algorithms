# algorithms

### 1. Reverse a string:

Five Ways 

__1. For loop__

```function reverse(str){
  let reversed = "";    
  for (var i = str.length - 1; i >= 0; i--){        
    reversed += str[i];
  }    
  return reversed;
}```

With Es6:
```function reverse(str){
  let reversed = "";
  for(let char of str){
    reversed = char + reversed;
  }
  return reversed;
}```

__2. reverse() Method for Arrays


