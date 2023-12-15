# ## **Getting started**

Given the following HTML:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Document</title>
  </head>
  <body>
    <div class="header"></div>
    <section id="container">
      <ul>
        <li class="first">one</li>
        <li class="second">two</li>
        <li class="third">three</li>
      </ul>
      <ol>
        <li class="first">one</li>
        <li class="second">two</li>
        <li class="third">three</li>
      </ol>
    </section>
    <div class="footer"></div>
  </body>
</html>
```

## **Exercise**

Write the code necessary to do the following:

1. Select the section with an id of container without using querySelector.
   ```js
   document.getElementById("container");
   ```
2. Select the section with an id of container using querySelector.
   ```js
   document.querySelector("#container");
   ```
3. Select all of the list items with a class of “second”.
   ```js
   document.querySelectorAll("li.second");
   ```
4. Select a list item with a class of third, but only the list item inside of the ol tag.
   ```js
   document.querySelector("ol > li.third");
   ```
5. Give the section with an id of container the text “Hello!”.
   ```js
   document.querySelector("#container").innerText = "Hello!";
   ```
6. Add the class main to the div with a class of footer.
   ```js
   document.querySelector(".footer").classList.add("main");
   ```
7. Remove the class main on the div with a class of footer.
   ```js
   document.querySelector(".footer").classList.remove("main");
   ```
8. Create a new li element.
   ```js
   const newLi = document.createElement("li");
   ```
9. Give the li the text “four”.
   ```js
   newLi.innerText = "four";
   ```
10. Append the li to the ul element.
    ```js
    document.querySelector("ul").appendChild(newLi);
    ```
11. Loop over all of the lis inside the ol tag and give them a background color of “green”.
    ```js
    for (elem of document.querySelector("ol").children) {
      elem.style.backgroundColor = "green";
    }
    ```
12. Remove the div with a class of footer
    ```js
    document.querySelector(".footer").remove();
    ```
