## DOM Assignment 8

### Task 1 : Make the right div "scrollable"

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
