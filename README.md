# My Bug Collection

## JavaScript

<details>
<summary> <h3>Can not read property of undefined</h3> </summary>
<ul style="list-style-type: none">
<li style="list-style: none"></li>
  <details> <summary>The Problem</summary>
  <p>when ever we see the word `property` in JavaScript it means we are refering to an object. We are trying to access a property from somthing that is not an object and thus, does not have properties.</p>
  </details>
</li>
<li>
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
</li>
</ul>
</details>





  