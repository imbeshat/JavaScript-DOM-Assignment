## DOM Assignment 5

### Task 1 : Add a "Pro Subscribtion" button, a new quick link named "Chinese" and a 6th recipe card

![image](https://user-images.githubusercontent.com/48837703/215987271-e965a933-664a-4961-983e-dcae1d3236af.png)

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

let parentGallery = document.querySelector(".recipe-gallery");

// code for creating and appending new recipe card div
let newCard = document.createElement("div");
newCard.className = "card";
parentGallery.appendChild(newCard);

//code for creating anchor tag inside new card and appending it
let newCardLink = document.createElement("a");
newCardLink.className = "recipe-text";
newCardLink.href = "#";
newCard.appendChild(newCardLink);

//code for creating img tag inside anchor and appending it
let newCardImage = document.createElement("img");
newCardImage.className = "recipe-img";
newCardImage.src = "https://www.brotherskitchen.in/wp-content/uploads/2021/03/chatpata-paneer-pizza-300x300.jpg";
newCardLink.append(newCardImage);

//code for creating h5 tag inside anchor and appending it
let newCardName = document.createElement("h5");
newCardName.className = "recipe-name";
newCardName.innerText = "Pizza";
newCardLink.append(newCardName);

//code for creating p tag inside anchor and appending it
let newCardDesc = document.createElement("p");
newCardDesc.className = "recipe-disp";
newCardDesc.innerText = "Prep : 15min | Cook : 30min";
newCardLink.append(newCardDesc);
```
