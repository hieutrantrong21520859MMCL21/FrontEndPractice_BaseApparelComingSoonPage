# Frontend Mentor - Base Apparel coming soon page

## 1. Overview

The challenge is to build out this Interactive rating component and get it looking as close to the design as possible.
Users should be able to:
- View the optimal layout for the interface depending on their device's screen size.
- See hover and focus states for all interactive elements on the page.
- Receive an error message when the form is submitted if:
  - The **input** field is empty.
  - The email address is not formatted correctly.

![Design preview for the Interactive rating component coding challenge](./design/desktop-preview.jpg)

### a) My screenshot

![My screenshot](./screenshot.jpeg)

### b) Links

- Solution URL: [my source code here](https://github.com/hieutrantrong21520859MMCL21/FrontEndPractice_Intern_BaseApparelComingSoonPage)
- Live Site URL: [my website's URL here](https://hieutrantrong21520859mmcl21.github.io/FrontEndPractice_Intern_BaseApparelComingSoonPage/)

## 2. My process

### a) Built with

- HTML
- CSS
- JavaScript
- Mobile - first workflow

### b) What I learned

- How to use _form_ element in HTML.
- How to apply _RegEx_ in form validation.
- Some codes I am most proud of (which consist of knowledge I have learned):

```html
<form action="">
  
  <input type="text" id="email" placeholder="Email Address">

  <input type="submit" value="" id="submit">
    
</form>
```

```javascript
const form = document.querySelector("form");
const email_input = document.getElementById("email");
const submit_btn = document.getElementById("submit");

const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;

form.addEventListener("submit", function (event) {

  if (!email_input.value.match(pattern)) {

    event.preventDefault();
    form.classList.add("invalid");
  }

});
```

### c) Useful resources

- [MDN - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML): this helped me a lot about HTML via articles.
- [Learn HTML](https://web.dev/learn/html): this is an amazing website that provides lessons about HTML with examples.
- [MDN - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS): this helped me well with CSS via articles.
- [Learn CSS](https://web.dev/learn/css): this is an amazing website that provides lessons about CSS with examples.
- [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript): this website a lot of useful articles.
- [javascript.info](https://javascript.info/): this website provides lots of lessons and detailed explanation.