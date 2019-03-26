### TypeScript

- `tsc`is the compiler. Usage: `tsc file.ts`.
- Watch mode: `tsc file.ts -w`.

##### Defining variable types.

```TypeScript
let my_string: string;
let my_num: number;
let my_bool: boolean;
let my_var: any;

let str_arr: string[];  // Forces the array to only accept strings.
let str_arr: Array<string>;  // Alternative syntax.
str_arr = ["Hello", "World"];

```

##### Tuple Useage

```TypeScript
let str_num_tuple: [string, number];
str_num_tuple = ["Hello", 4, 3, 4];
```
