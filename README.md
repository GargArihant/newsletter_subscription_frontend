# Frontend Mentor - Newsletter sign-up form with success message solution

This is a solution to the [Newsletter sign-up form with success message challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/newsletter-signup-form-with-success-message-3FC1AZbNrv). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- Add their email and submit the form
- See a success message with their email after successfully submitting the form
- See form validation messages if:
  - The field is left empty
  - The email address is not formatted correctly
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![Screenshot](./assets/images/Screenshot%202023-07-10%20145007.png)


### Links

- Solution URL: [solution URL](https://github.com/GargArihant/newsletter_subscription_frontend)
- Live Site URL: [live site URL](https://clever-cassata-388fc7.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- JavaScript DOM manipulation



### What I learned

During this project I learned a lot about html Forms and how to use Javascript to display error messages based on different scenarios and the correct order to use them.


```js
function validateForm() {
            let email = document.getElementById('email');
            let error = document.getElementById('error');
        let y = document.forms['myForm']['email'].value;
            if (y == '') {
               
            email.style.cssText= 'border: 1px solid red; background-color: rgba(255, 0, 0, 0.122)' ;
            error.style.cssText='display: inline; color: red; position: absolute; top: 0; right: 10px; font-size: 12px';
            return false;
            }
        else if (y.match(/^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$/)) {
            return true;
        } else {
            email.style.border= '1px solid red';
            error.style.cssText='display: inline; color: red; position: absolute; top: 0; right: 10px; font-size: 12px';
            return false;
        }
        }
```

### Continued development

I would like to continue working on more CSS responsive layout designs and how they can be made more flexible and with less code duplication.

### Useful resources

- (https://www.w3schools.com/js/js_validation.asp) - This helped me in setting up the error states for form validation uing javascript dom manipulation.
- (https://stackoverflow.com/questions/22607150/getting-the-url-parameters-inside-the-html-page) - There are some good answers here about how to excess url params easily through Javascript APIs.


## Author

- Website - [Arihant Garg](https://github.com/GargArihant)
- Frontend Mentor - [@GargArihant](https://www.frontendmentor.io/profile/GargArihant)
- LinkedIn - [Arihant Garg](www.linkedin.com/in/
arihant-garg-631a68208)

