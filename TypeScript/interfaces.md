### Interfaces

- Without Interface.

```TS
function show_todo(todo: {title: string, text: string}){
  console.log(todo.title+": "+todo.text);
}

let my_todo = {title: "Trash", text: "Take out trash"}

show_todo(my_todo);
```

- With Interface.

```TS
interface Todo{
  title: string;
  text: string;
}

function show_todo(todo: Todo}){
  console.log(todo.title+": "+todo.text);
}

let my_todo = {title: "Trash", text: "Take out trash"}

show_todo(my_todo);
```