## Assignmet 1

### Task 1 : Add "Hire Me" in nav bar

![image](https://user-images.githubusercontent.com/48837703/215449066-347e1572-0fe4-4efb-a024-366618a3a591.png)

### Solution

```
let parentUl = document.querySelector("ul");
let hireMeLi = document.createElement("li");
hireMeLi.innerHTML = `<a href="#">Hire Me</a>`;
parentUl.appendChild(hireMeLi);
```

### Task 2 : Change the placeholder value in search to "Search My Project"

![image](https://user-images.githubusercontent.com/48837703/215451474-e71ce622-4dc5-4c41-8f0b-e54d035a094b.png)

### Solution

```
let newPlaceholder = document.querySelector("input");
newPlaceholder.placeholder = "Search My Project";
```

### Task 3 : Change "a Freelancer" to "an Employee" and "National and International Client" to iNeuron Intelligence Pvt Ltd"

![image](https://user-images.githubusercontent.com/48837703/215527128-a8b9ce1f-9fa5-4f46-8d69-8d7d67b196fd.png)

```
let spanElement = document.querySelectorAll(".hero-left-section p span");
spanElement[1].innerText = "an Employee";
spanElement[2].innerText = "iNeuron Intelligence Pvt Ltd";
```

### Task 4 : Add the image in the avatar

![image](https://user-images.githubusercontent.com/48837703/215529728-a26d78f5-da9d-4a84-b4b7-cced4cb64bb5.png)

```
let image = document.querySelector(".hero-right-section img");
image.src = "https://hiteshchoudhary.com/static/a8d73d1aac4c79e9bb689640e6090367/2eaab/person-image.jpg";
```
