## DOM Assignment 8

### Task 1 : Make the right div "scrollable"

![image](https://user-images.githubusercontent.com/48837703/216286658-c8b88ab6-4a80-4920-ac51-47ae8ea5d13d.png)

### Solution

```
// code for making div scrollable
let scrollNew = document.querySelector("aside");
scrollNew.style.overflowY = "scroll";

// adding border
scrollNew.style.border = "3px solid red";

// code for adding new heading and paragraph
// adding and appending hr
let newHr = document.createElement("hr");
scrollNew.appendChild(newHr);
newHr.className = "hr-line";

// code for adding and appending new heading
let newHeading = document.createElement("h2");
newHeading.className = "new-head";
newHeading.innerText = "This is Custom Heading";
scrollNew.appendChild(newHeading);

// code for adding and adding new paragraph
let newPara = document.createElement("p");
newPara.className = "new-p";
newPara.innerText = "Custom Paragraph. Lorem ipsum paraghrap. We take Lorem ipsum as input.";
scrollNew.appendChild(newPara);

```

### Task 2 : Remove background image form body

![image](https://user-images.githubusercontent.com/48837703/216287715-a5f07f7c-3def-4578-91c1-74c5765e2f62.png)

### Solution

```
let body = document.querySelector("body");
body.style.backgroundImage = "none";
```

### Task 3 : add event listener to hamburger icon

![image](https://user-images.githubusercontent.com/48837703/216383319-a5b23cc1-c2d5-4535-b9f0-0313d8f5d93f.png)

### Solution

```
// code for making hamburger icon responsive
let hamBtn = document.querySelector(".navbar-toggler-icon");

hamBtn.addEventListener("click", () => {
  let navItems = document.querySelector("#navbarTogglerDemo01");
  if (navItems.style.display === "block") {
    navItems.style.display = "none";
  } else {
    navItems.style.display = "block";
  }
});
```
