# My Bug Collection

## JavaScript

<details>
<summary> Uncaught TypeError: Cannot read property 'foo' of undefined </summary>
  <ul>
  <li>
    <details><summary>The Problem</summary>
    <p> Whenever we see the word <code>property</code> in JavaScript it means we are refering to an object and that we are probably using dot notation. In this error it is telling us that we are trying to access a property from a variable that is not an object and thus. That is why the error starts with <code>TypeError</code>. It is telling us that the data behind the variable is not the data that we expected.</p>
    </details>
  </li>
  <li>
  <details>
  <summary>Example</summary>

  ```js
  var obj = {
  name: "Bob Ross",
  age: 52
  }

  // We get the value we expected when accessing obj.name
  console.log(obj.name); // Bob Ross

  // Here we try and access the property 'childred' from obj, because it does not have that property it resolves into 'undefined'
  console.log(obj.children) // undefined

  // Because  'obj.children' is 'undefined' trying to access a propery off of it will actaully break JavaScript.
  console.log(obj.children.first) // ERROR: cannot read property first of undefinded

  // when the above line resolves, it actually looks like this.
  console.log(undefined.first)

  ```

  </details>
  </li>
  <li>
  <details><summary>Aproaches to Fix</summary>
    <h3>Common Assumptions</h3>
    <p>A common assumption that gets made is thinking that you know what the strucure of the data is, and all the properties on the object. When getting this error it is important to understand that the word 'foo' is not the issue. its the propertie that came before that really is the root if the issue. This can be confusing becaue the console is telling you the value of the property, but not the name of the property that caused the issue. Meaning the undefined is the issue, not 'foo'  (property 'foo' of undefiend).</p>
    <h4>Tactics</h4>
    <ul>
      <li>
       If you were accessing data from an object like this <code>obj.children.first</code>, a good idea can be to console.log the most left value <code>obj</code> and compare it to your assumptions of what you expect to see. Then console.log the next value <code>obj.children</code>, and keep doing this until you find what value is undefined.
      </li>
      <li>
        A problem of being human is that we often automatically fix mistakes in typing or spelling without realizing that we do it. Make sure when you are reading over your object chain that you are reading character by character, not word by work. If you get in the habbit of doing this your time to finding typos will drop dramatically
      </li>
    </ul>
  </details>
  </li>
    <li>
  <details><summary>Related Issues</summary>
    <ul>
      <li>React: cannot read property SetState of undfined | null</li>
    </ul>
  </details>
  </ul>
</ul>
</details>



<details>
<summary> Uncaught TypeError: foo.baz is not a function </summary>
  <ul>
  <li>
    <details><summary>The Problem</summary>
    <p> This is another type error, meaning that you are not working with the dataType that you expected.</p>
    </details>
  </li>
  <li>
  <details>
  <summary>Example</summary>

  ```js
  var obj = {
  name: "Bob Ross",
  age: 52
  }

  // We get the value we expected when accessing obj.name
  console.log(obj.name); // Bob Ross

  // Here we try and access the property 'childred' from obj, because it does not have that property it resolves into 'undefined'
  console.log(obj.children) // undefined

  // Because  'obj.children' is 'undefined' trying to access a propery off of it will actaully break JavaScript.
  console.log(obj.children.first) // ERROR: cannot read property first of undefinded

  // when the above line resolves, it actually looks like this.
  console.log(undefined.first)

  ```

  </details>
  </li>
  <li>
  <details><summary>Aproaches to Fix</summary>
    <h3>Common Assumptions</h3>
    <p>A common assumption that gets made is thinking that you know what the strucure of the data is, and all the properties on the object. When getting this error it is important to understand that the word 'foo' is not the issue. its the propertie that came before that really is the root if the issue. This can be confusing becaue the console is telling you the value of the property, but not the name of the property that caused the issue. Meaning the undefined is the issue, not 'foo'  (property 'foo' of undefiend).</p>
    <h4>Tactics</h4>
    <ul>
      <li>
       If you were accessing data from an object like this <code>obj.children.first</code>, a good idea can be to console.log the most left value <code>obj</code> and compare it to your assumptions of what you expect to see. Then console.log the next value <code>obj.children</code>, and keep doing this until you find what value is undefined.
      </li>
      <li>
        A problem of being human is that we often automatically fix mistakes in typing or spelling without realizing that we do it. Make sure when you are reading over your object chain that you are reading character by character, not word by work. If you get in the habbit of doing this your time to finding typos will drop dramatically
      </li>
    </ul>
  </details>
  </li>
    <li>
  <details><summary>Related Issues</summary>
    <ul>
      <li>React: cannot read property SetState of undfined | null</li>
    </ul>
  </details>
  </ul>
</ul>
</details>
