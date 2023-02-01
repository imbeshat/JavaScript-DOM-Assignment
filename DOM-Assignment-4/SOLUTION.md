## DOM Assignment 4

### Task 1 : Change the name of the Character 2 to "The Archer" & Character 4 to "The Goblin". Also change the the color each character card stats.

![image](https://user-images.githubusercontent.com/48837703/215792352-f896fa94-e64f-4c75-838f-01b100d3002c.png)

### Solution

```
// code to change the name of the Character 2 to "The Archer"
let archer = document.querySelectorAll(".archer div");
archer[2].innerText = "The Archer";

// code to change the name of the Character 4 to "The Goblin"
let goblin = document.querySelectorAll(".goblin div");
goblin[2].innerText = "The Goblin";

// code to change the color of the stats section of each charcter card
let barbarianColor = document.querySelector(".clash-card__unit-stats--barbarian");
barbarianColor.style.backgroundColor = "#ec9b3b";

let archerColor = document.querySelector(".clash-card__unit-stats--archer");
archerColor.style.backgroundColor = "#ee5487";

let giantColor = document.querySelector(".clash-card__unit-stats--giant");
giantColor.style.backgroundColor = "#f6901a";

let goblinColor = document.querySelector(".clash-card__unit-stats--goblin");
goblinColor.style.backgroundColor = "#82bb30";

let wizardColor = document.querySelector(".clash-card__unit-stats--wizard");
wizardColor.style.backgroundColor = "#4facff";

// code to change the font color of the stats section of each charcter card
let fontColorAll = document.querySelectorAll(".one-third");
fontColorAll.forEach((e)=>{
    e.style.color = "#fff";
})
```
