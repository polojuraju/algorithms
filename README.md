# algorithms

### 1). Reverse a string in js:

Five Ways 

__i. For loop__

``` function reverse(str){
  let reversed = "";    
  for (var i = str.length - 1; i >= 0; i--){        
    reversed += str[i];
  }    
  return reversed;
}
```

With Es6:
```function reverse(str){
  let reversed = "";
  for(let char of str){
    reversed = char + reversed;
  }
}
```

__ii. reverse() Method for Arrays__
```function reverse(str){
  return str.split("").reverse().join("");
}
```
__iii. Spread Syntax (ES6) + reverse() Method for Arrays__
```function reverse(str){
  return [...str].reverse().join('');
}
```
__iv. reduce() Method for Arrays
```
function reverse(str){
  return str.split("").reduce((rev, char)=> char + rev, ''); 
}
```
v.Recursion
```
function reverse(str){
 if(str === ""){
  return str 
 }else{
  return reverse(str.substr(1)) + str[0]
 }
}
(or)
function reverse(str){
 return str ? reverse(str.substr(1)) + str[0] : str
}
```

