# My Bug Collection

## JavaScript

<details>
  <summary>Can not read property of undefined | null<summary/>
  <h3>The Problem</h3>
  <p>when ever we see the word `property` in JavaScript it means we are refering to an object. We are trying to access a property from somthing that is not an object and thus, does not have properties.</p>
  <h4>Example</h4>

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