## DOM Assignment 9

### Task 1 : Change the color of h1 to red and add the cart icon

![image](https://user-images.githubusercontent.com/48837703/216388958-f1118de7-164d-43d5-be9b-42dea885dea2.png)

### Solution

```
// code for chaanging the color of h1
let heading = document.querySelector("h1");
heading.style.color = "#dc143c";

//code for adding the cart icon
let cartImg = document.querySelector("button img");
cartImg.src = "./images/icon-cart.svg";
```

### Task 2 : Change the color of "Add to Cart" button and add the cart icon

![image](https://user-images.githubusercontent.com/48837703/216390416-b0b985ca-1613-4e88-a9a9-eb2e687661d6.png)

### Solution

```
// code for changing the color of "Add to Cart" button
let cartBtn = document.querySelector("button");
cartBtn.style.backgroundColor = "#dc143c";

//code for adding the cart icon
let cartImg = document.querySelector("button img");
cartImg.src = "./images/icon-cart.svg";
```
