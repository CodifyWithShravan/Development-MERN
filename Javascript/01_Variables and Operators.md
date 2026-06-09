- Javascript is a scripting or interpreted programming language used to make the webpages interactive and implement complex features on the webpage.
- `console.log()` --> It is used to print something to the dev console in the browser
- To link javascript file externally we do by writing this below syntax in the head tag of the html.

```html
<script src="javascript.js"></script>
```
  
## Variables 

- It is like the storage containers for the data.
- Variables are declared by the keyword `let` .
  
```javascript
let firstname = "shravan";
let lastname = "Kumar";
console.log(firstname);
console.log(lastname);
```

- We can reassign the variables while using the `let` keyword.
- `const` keyword is used to permanently assign value to the variable so that it cannot be reassigned
  
```javascript
const pi = 3.14;
console.log(pi); // gives the output 3.14
pi = 4;
console.log(pi); // gives an error that using const keyword cannot be reassigned.
```

- Javascript follows the **BODMAS** or **PEMDAS** order of operations.
- API are generally are of two types
  1. Browser API's
  2. Third party API's
 
- When the browser detects the javascript block it runs in an order that is from top to bottom.
```javascript
function updateName() { // updateName() is called a function(reusable blocks)
  const name = prompt("Enter a new name");
  button.textContent = `Player 1: ${name}`;
}

const button = document.querySelector("button"); // we store the reference to a button 

button.addEventListener("click", updateName); // This calls the function updateName when the button is clicked
```

The above code is executed from the top to bottom. If we move the addEventListener to the top the button will not work and does not call the function.

> [!Note]
>**Hoisting** : The process where the interpreter moves the declaration of the functions, variables, classes , or imports to the top of the scope before the execution of the code.
>
>**Intrepreted language** : The code is run from the top to bottom and the result is immediately returned.


 - Javascript interpreter uses the **Just-In-Time** compiling to improve the performance.

### Strategies to make sure that javascript runs only after the HTML is parsed

- In the internal Javascript the script tag is kept at the bottom of the body so that it loads at the last and the HTML is rendered first.
- In the external Javascript the script element should be kept in the head tag and should use the attribute `type = "module` so that the code is treated as module and browser waits for all the HTML is parsed before executing the Javascript modules.

## Numbers

```javascript
let myNumber = "69";
typeof(myNumber); // gives type string
myNumber = Number(myNumber);
typeof(myNumber); // now gives the type number
```

## Operators

| Operator | Name                  |
| -------- | --------------------- |
| `+`      | Addition              |
| `-`      | Subtraction           |
| `*`      | Multiplication        |
| `/`      | Division              |
| `%`      | Remainder<br>(Modulo) |
| `**`     | Exponent              |

## Assignment Operators

| Operator | Name                         |
| -------- | ---------------------------- |
| `+=`     | Addition<br>Assignment       |
| `-=`     | Subtraction<br>Assignment    |
| `*=`     | Multiplication<br>Assignment |
| `/=`     | Division<br>Assignment       |

## Comparison Operators

| Operator | Name                                 |
| -------- | ------------------------------------ |
| `===`    | Strict Equality(Checks datatype too) |
| `!==`    | Strict non equality                  |
| `<`      | Less than                            |
| `>`      | Greater than                         |
| `<=`     | Less than or equal to                |
| `>=`     | Greater than or equal to             |
| `==`     | Equality                             |
| `!=`     | Not equality                         |

## String Concatenation (Binary form)

- For joining the strings we use `+` operator.
```javascript
let s = "shravan" + "Kumar";
console.log(s); // mystring
```

- If any of the operand is string, then another converts into string.
```javascript
console.log('1' + 2); // "12"
console(2 + "1"); // "21"
```

```javascript
console.log(6 - "2"); // 4, converts "2" to a number
console.log("6" / "2"); // 3, converts both operands to number
```

## Numeric Conversion (Unary form)

- Unary operator `+` converts which is not a number into a number
- It does the same as the `Number()` but in a shorter way.

```javascript
let oranges = "2";
let mangoes = "5";
console.log(oranges)
console.log(mangoes)
console.log(oranges + mangoes) // "25"
console.log(+oranges + +mangoes) // both values are converted into numbers. output: 7
```
