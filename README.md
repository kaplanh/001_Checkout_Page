
# Checkout_Page


![checkoutpage](https://github.com/kaplanh/Checkout_Page/assets/101884444/5cfce62d-d646-4ca7-8f0c-d7a58be1d7b3)


[Click Me!](https://kaplanh.github.io/Checkout_Page/)

## Description

The project aims to create a Checkout App using JS and Bootstrap.

## Problem Statement

- Your company has recently started on a project that aims to create a Checkout App. So you and your colleagues have started to work on the project.

## Project Skeleton 

```
Checkout App (folder)
|
|----readme.md                        
|----index.html
|----style.css
|----app.js
|----img (folder)
``` 


### At the end of the project, the following topics are to be covered;

- HTML
  - font-awesome 
   ```
     <link
            rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
            integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw=="
            crossorigin="anonymous"
            referrerpolicy="no-referrer"
        />
   
   ```
 
-CSS
 - Nested CSS
 - text-decoration: line-through
 ```
    .nav__list--btn {
    color: orangered;
    font-size: 14px;
    cursor: pointer;

    & i:hover {
        color: white;
        border-radius: 50%;
        background-color: #ff7623;
    }
    }

.line-through {
    text-decoration: line-through;
}
   
   ```
- @media query

 ```
@media only screen and (max-width: 1150px) {
    .nav__list {
        padding: 0rem 1rem;
    }
  ```
  
  
- JS
  - DOM Manipulations
    - innerHTML
    - innerText
    - textContent
     
  - DOM Selectors
  - querySelector
  - querySelectorAll
  - const productList = document.querySelector("div.main__product-painel"); //?basina div yazarak belirtirsek performans acisindan daha hizli olur
    
  - Events
    - click
    - load
  
  -e.target & e.currentTarget
    ```
         e.currentTarget.firstElementChild.innerText = "My Cart";
        //? NOT:e.target tiklanan elementi verirken e.currentTarget sabittir ve addEventListener in tanimlandigi elemandir burda navbarList  ve daha hizlidir
    ```
  - Capturing & Bubbling
  - DOM Traversing
    - nextElementSibling
    - nextElementSibling
    - e.target.closest(".main__product-info")
    - if (e.target.classList.contains("fa-plus"))
    - e.target.previousElementSibling.innerText++;
    - firstElementChild
    - children
   
  - localStorage & sessionStorage
 
  
  - Array Methods
  - forEach() & reducer()
     ```
     forEach() ==> array, nodeList te calisir
    let subtotal = 0;
    productPriceDivs.forEach((price) => {
        subtotal += parseFloat(price.innerText);
    });
    console.log(subtotal);
    ```
 
      ```
    reduce()
    const subTotalAlternatif = [...productPriceDivs]; //reduce icin array a dönüstürmeliyiz
    let subtotal = subTotalAlternatif.reduce((acc, curr) => {
        return acc + parseFloat(curr.innerText); //parseFloat  stringten float yapar
    }, 0);

    ```
  
  - parseFloat
    ```
    const taxPrice = parseFloat(subtotal * localStorage.getItem("taxRate")); parseFloat  stringten float yapar

    ```

  
  - if else - if - else  conditions
  - Ternary
    ```
     subTotal 3000 den büyükse shippingPrice 0 olmasi icin
      const shippingPrice =
          subtotal > 0 && subtotal < localStorage.getItem("freeShippingPrice")
              ? parseFloat(localStorage.getItem("shippingPrice"))
              : 0; //localStorage den gelen veriler string olarak gelir

    ```
 
 
     

  - String Methods( toFixed() )
   ```
   <td>${(taksit * vade.value).toFixed(2)} ₺</td>
  ```

    

### At the end of the project, developers will be able to;

- improve coding skills within HTML, CSS and JS 

- use git commands (push, pull, commit, add etc.) and Github as a Version Control System.


## Notes

- You can use HTML, CSS and JS to complete this project.



<p align="center"> ⌛<strong> Happy Coding </strong> ✍ </p>




