## DOM Assignment 5

### Task 1 : Add a "Pro Subscribtion" button, a new quick link named "CHinese" and a 6th recipe card

```
// code for adding a "Pro Subscribtion" button
let parentDiv = document.querySelectorAll(".nav-center div");

let btnPro = document.createElement("a");
btnPro.innerText = "Pro Subscription";
btnPro.className = "btn";
btnPro.href = "#";

parentDiv[2].appendChild(btnPro);

// code for adding a new quick link named "Chinese"
let parentLinkDiv = document.querySelector(".tags-container div");

let chineseLink = document.createElement("a");
chineseLink.href = "#";
chineseLink.innerText = "Chinese (7)";

parentLinkDiv.appendChild(chineseLink);
<a href=​"#">​Chinese (7)​</a>​
```
