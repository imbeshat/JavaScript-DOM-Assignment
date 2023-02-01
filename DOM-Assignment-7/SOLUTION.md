## DOM Assignment 7

### Task 1 : Remove the languages that have 2.0 in their name(Every alternative language)

![image](https://user-images.githubusercontent.com/48837703/216105274-3a8ace3a-a14a-4d9e-992e-8740d503a249.png)

### Solution

```
let altLanguage = document.querySelectorAll(".main__languages a:nth-child(2n)");
altLanguage.forEach((language)=>{
    language.style.display="none";
});
```

### Task 2 : Use JavaScript to write something in the input box and submit the form. This should refresh the page and the languages in the left card should come back.

Before Clicking Submit:
![image](https://user-images.githubusercontent.com/48837703/216134857-ed75d8a3-e3f9-4466-9d3e-08d128fe15d0.png)

After Clicking Submit:
![image](https://user-images.githubusercontent.com/48837703/216135402-341ce3fd-a788-4ef5-a383-e6d2189b6a32.png)

```
let input = document.querySelector("input");

// entering the value of input
input.value = "iNeuron";

// enabling the submit button
document.querySelector(".main__form-btn").disabled = false;

// adding event listener to submit the value
let btnSubmit = document.querySelector(".main__form-btn");
btnSubmit.addEventListener("submit", (e)=>{
    e.preventDefault();
    window.location.reload();
});
```
