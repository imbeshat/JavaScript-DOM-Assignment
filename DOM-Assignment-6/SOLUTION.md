## DOM Assignment 5

### Task 1 : Change equalizer logo to iNeuron logo

![image](https://user-images.githubusercontent.com/48837703/216009092-26711fae-2506-4581-a666-3cdc7c6915dd.png)

### Solution

```
let logoImg = document.querySelector("header img");
logoImg.src = "./assets/ineuron-logo.png";
```

### Task 2 : Change $4 to "$10" in pricing

![image](https://user-images.githubusercontent.com/48837703/216010422-09c3a292-bb56-4b7b-831d-4a288b46b8a7.png)

### Solution

```
let appPrice = document.querySelector(".app_price span");
appPrice.innerText = "$10";
```
