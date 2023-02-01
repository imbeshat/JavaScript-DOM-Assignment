## DOM Assignment 5

### Task 1 : Change equalizer logo to iNeuron logo

![image](https://user-images.githubusercontent.com/48837703/216009092-26711fae-2506-4581-a666-3cdc7c6915dd.png)

### Solution

```
let logoImg = document.querySelector("header img");
logoImg.src = "./assets/ineuron-logo.png";
```

### Task 2 : Change $4 to "$10" in pricing

![image](https://user-images.githubusercontent.com/48837703/216015377-6ad75f0c-0f0a-4226-a0c3-2241264d0797.png)

### Solution

```
// code for changing the app price
let appPrice = document.querySelector(".app_price span");
appPrice.innerText = "$10";

let socialIcon = document.querySelector(".footer_social");

// creating linkedin div and appendind it
let linkedinDiv = document.createElement("div");
linkedinDiv.className = "footer_social_ico";
socialIcon.appendChild(linkedinDiv);

// creating linkedin icon and appending it
let linkedinIcon = document.createElement("i");
linkedinIcon.classList = "fa-brands fa-linkedin";
linkedinDiv.appendChild(linkedinIcon);
```
