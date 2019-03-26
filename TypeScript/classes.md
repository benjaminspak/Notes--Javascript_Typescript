### Classes

```TS
class User {  // Creating the class.
  name: string;
  email: string;
  age: number;

  constructor(name: string, email: string, age: number;){
    this.name = name;
    this.email = email;
    this.age = age;

    console.log("User Created: "+this.name);
  }

  register(){
    console.log(this.name+" is now registered");
  }
}

// Instantiating the class.
let john = new User("John Doe", "jdoe@gmail.com", 34);

console.log(john.age);

john.register();
```

##### Access Modifiers

- Public: can be accessed by instances of class - Use case: API.
- Private: cannot be access by an instance of the class.
- Protected: Cannot be accessed from outside the class. But, can be accessed from any class that inherits the original class.

##### Inheritance

```TS
class User {  // Creating the class.
  name: string;
  email: string;
  age: number;

  constructor(name: string, email: string, age: number){
    this.name = name;
    this.email = email;
    this.age = age;

    console.log("User Created: "+this.name);
  }

  register(){
    console.log(this.name+" is now registered");
  }

  pay_invoice(){
    console.log(this.name+" paid invoice");
  }
}

class Member extends User(){
  id: number;

  constructor(id: number, name: string, email: string, age: number){
    super(name, email, age);
    this.id = id;
  }

  pay_invoice(){
    super.pay_invoice()
  }
}

let mike: User = new Member(1, "Mike Smith", "mikes@gmail.com" 33);
```