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
