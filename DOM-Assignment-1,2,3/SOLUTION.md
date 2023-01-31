## DOM Assignmet 1

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

### Task 5 : Add a button named "Support Me" below the avatar

![image](https://user-images.githubusercontent.com/48837703/215531933-e9e4fc68-9161-4124-8cbf-94dbcf4f782d.png)

```
let btn = document.querySelector(".hero-right-section-btns");
let btnSupport = document.createElement("button");
btnSupport.innerText = "Support Me";
btn.appendChild(btnSupport);
```

## DOM Assignment 2

### Task 1 : Change the color of accordian and their paragraphs

![image](https://user-images.githubusercontent.com/48837703/215551263-1b8a8286-6a6e-4b0a-99a1-8d5e3be21419.png)

```
let accordianHeading = document.querySelectorAll(".accordian h3");
let accordianPara = document.querySelectorAll(".accordian p");
accordianHeading.forEach((head)=>{
    head.style.backgroundColor = "#dadaf8";
});
accordianPara.forEach((para)=>{
    para.style.backgroundColor = "#eeeeff";
});
```

### Task 2 : Add a new accordian named "Skills" to the end of the list and change the color again

![image](https://user-images.githubusercontent.com/48837703/215706443-20efaf4f-c6c3-4372-81f8-8ecbd2cbc112.png)

```
// code for appending new accordian to the end of the list
let parentAcc = document.querySelector(".accordian-wrapper");

let newAccordian = document.createElement("div");
newAccordian.classList.add("accordian");

let accordianHead = document.createElement("h3");
accordianHead.innerText = "Skills";

let accordianPara = document.createElement("p");
accordianPara.innerText = "I posses a very good command over the Full Stack Development technologies like MERN which can be seen in my work over the Github."
accordianPara.style.display = "none";

parentAcc.appendChild(newAccordian);
newAccordian.appendChild(accordianHead);
newAccordian.appendChild(accordianPara);

// code for adding event listener for the new accordian
let accordianDrop = document.querySelectorAll(".accordian h3");
accordianDrop[accordianDrop.length-1].addEventListener("click", (element) => {
    let para = element.target.nextElementSibling;
    if (para.style.display === "block") {
        para.style.display = "none";
    } else {
        para.style.display = "block";
    }
});

// code for changing accordian color
let accordianHeading = document.querySelectorAll(".accordian h3");
let accordianPara = document.querySelectorAll(".accordian p");
accordianHeading.forEach((head)=>{
    head.style.backgroundColor = "#dadaf8";
});
accordianPara.forEach((para)=>{
    para.style.backgroundColor = "#eeeeff";
});
```

## DOM Assignment 3

### Task 1 : Add event listener to the inputs of "User Input Board" and send the data to the inputs of "User Output Board"

![image](https://user-images.githubusercontent.com/48837703/215722534-1a522e56-ae6b-4a70-ba8a-9f2b09d3e6ef.png)

```
// Selecting input box of User Input Board
let getName = document.querySelector(".userName");
let getEmail = document.querySelector(".userEmail");
let getMessage = document.querySelector(".userMessage");

// Selecting input box of User Output Buard
let setName = document.querySelector(".enterName");
let setEmail = document.querySelector(".enterMail");
let setMessage = document.querySelector(".enterMessage");

// code for Submit button
let btnSubmit = document.querySelector(".mainRight form button");
btnSubmit.addEventListener("click",(e)=>{
    e.preventDefault();

    // Setting the value of User Output Board
    setName.value = getName.value;
    setEmail.value = getEmail.value;
    setMessage.value = getMessage.value;
});

// code for Reset button
let btnReset = document.querySelector(".mainLeft form button");
btnReset.addEventListener("click", (e)=>{
    e.preventDefault();

    // Clearing the value of User Output Board
    setName.value = "";
    setEmail.value = "";
    setMessage.value = "";

     // Clearing the value of User Input Board
    getName.value = "";
    getEmail.value = "";
    getMessage.value = "";
});
```
