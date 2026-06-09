# Data Types 

1. **Number** : It represents both integer and floating point numbers
   - `Infinity` 
     ```javascript
     console.log(1/0);
     console.log(Infinity) // also can be written like this
     ```
   - `NaN` : Not a number represents computational error which is caused by performing incorrect mathematic operations
     ```javascript
     console.log("not a number"/2); // NaN, such division doesn't exist
     console.log( NaN + 1 ); // NaN
     console.log( 3 * NaN ); // NaN
     console.log( "not a number" / 2 - 1 ); // NaN
     ```
     > [!NOTE]
     > `NaN ** 0` is `1` 
     
2. **BigInt** : Can safely represent larger values like in the range ±($2^{53}$-1).
   - This type is introduced to represent integers of arbitrary length.
     ```javascript
     //the "n" at the end means it's a BigInt
     const bigInt = 1234567890123456789012345678901234567890n;
     ```

3. **String** :  Characters surrounded within quotes whether it is double, single or backticks.
   - Double and single quotes are for: Simple quotes
   - Backticks are for extended functionality, that allow us to embed variables into the string by `${...}`, and are special kind of a string called `Template literal`.  
     ```javascript
     let str1 = "Hello";
     let str2 = 'Hello within single quotes';
     let str3 = `Can embed another variable like hey ${str1}`; // Can perform mathematical operation in it.
     ```

1. **Boolean** : Has two values `true` or `false`.

2. **Null** : It forms a seperate type which doesn't belong to any of the type and contains the null value
   - It just represents `nothing`, `empty` or `value unknown`.

6. **Undefined** : It makes a type of its own just like the `null` 
   - It means `value is not assigned` 
     ```javascript 
     let age;
     alert(age);
     ```

7. **Object** : These are used to store the collection of data and more complex entities.

8. **Symbol** : These are used to create unique identifiers for the objects

### Basic String Methods

| Methods |
| ------- |
| [String length](https://www.w3schools.com/js/js_string_methods.asp#mark_length) <br>[String charAt()](https://www.w3schools.com/js/js_string_methods.asp#mark_charat) <br>[String charCodeAt()](https://www.w3schools.com/js/js_string_methods.asp#mark_charcodeat) <br>[String codePointAt()](https://www.w3schools.com/js/js_string_methods.asp#mark_codepointat) <br>[String concat()](https://www.w3schools.com/js/js_string_methods.asp#mark_concat) <br>[String at()](https://www.w3schools.com/js/js_string_methods.asp#mark_at) <br>[String [ ]](https://www.w3schools.com/js/js_string_methods.asp#mark_propertyaccess) <br>[String slice()](https://www.w3schools.com/js/js_string_methods.asp#mark_slice) <br>[String substring()](https://www.w3schools.com/js/js_string_methods.asp#mark_substring) <br>[String substr()](https://www.w3schools.com/js/js_string_methods.asp#mark_substr) <br>[String toUpperCase()](https://www.w3schools.com/js/js_string_methods.asp#mark_touppercase) <br>[String toLowerCase()](https://www.w3schools.com/js/js_string_methods.asp#mark_tolowercase)<br>[String isWellFormed()](https://www.w3schools.com/js/js_string_methods.asp#mark_iswellformed) <br>[String toWellFormed()](https://www.w3schools.com/js/js_string_methods.asp#mark_towellformed) <br>[String trim()](https://www.w3schools.com/js/js_string_methods.asp#mark_trim) <br>[String trimStart()](https://www.w3schools.com/js/js_string_methods.asp#mark_trimstart) <br>[String trimEnd()](https://www.w3schools.com/js/js_string_methods.asp#mark_trimend) <br>[String padStart()](https://www.w3schools.com/js/js_string_methods.asp#mark_padstart) <br>[String padEnd()](https://www.w3schools.com/js/js_string_methods.asp#mark_padend) <br>[String repeat()](https://www.w3schools.com/js/js_string_methods.asp#mark_repeat) <br>[String replace()](https://www.w3schools.com/js/js_string_methods.asp#mark_replace) <br>[String replaceAll()](https://www.w3schools.com/js/js_string_methods.asp#mark_replaceall) <br>[String split()](https://www.w3schools.com/js/js_string_methods.asp#mark_split) |

## Comparisons
- The comparison operators return the boolean value.
### String Comparisons 
- Javascript uses `dictionary` or `lexicographical` order where the strings are compared letter-by-letter.