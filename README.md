# My Bug Collection

## JavaScript

<details>
<summary> Can not read property of undefined </summary>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<details> <summary>The Problem</summary>
  <p>when ever we see the word `property` in JavaScript it means we are refering to an object. We are trying to access a property from somthing that is not an object and thus, does not have properties.</p>
  </details>
  <details> <summary>Example</summary>

  ```JS
  var obj = {
    name: "Bob Ross",
    age: 52
  }

  console.log(obj.name); // Bob Ross
  console.log(obj.children) // undefined
  console.log(obj.children.first) // ERROR: cannot read property first of undefinded
  ```
  </details>
  
</details>





  