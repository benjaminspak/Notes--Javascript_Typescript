### TypeScript Functions

- Without TS.

```TS
function get_sum(num1, num2) {
  return num1 + num2;
}

console.log(get_sum(1,4));  // 5
```

- With TS.

```TS
function get_sum(num1:number, num2:number):number{  // Args are required to be ints & the return value must be an Int.
  return num1 + num2;
}

console.log(get_sum(1,4));  // 5
```

- Any Type.

```TS
let my_sum = function(num1:any, num2:any):number{
  if(typeof num1 == 'string'){
    num1 = parseInt(num1);
  }
    if(typeof num2 == 'string'){
    num1 = parseInt(num2);
  }
  return num1 + num2;
}

console.log(my_sum("3", 5));  // 8
```

- Optional.

```TS
function get_name(firstName:string, lastName:string):string{  // ? Makes the arg optional.
  if(lastName == undefined){
    return firstName;
  }
  return firstName+" "+lastName;
}

console.log()
```

- Void (not returning anything at all).

```TS
function my_void():void{
  return;
}
```
