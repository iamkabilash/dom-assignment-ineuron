# Dom Manipulation Assignment

# 1. Website Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)

## Answer
```
document.getElementsByClassName("crayons-subtitle-2 lh-tight mb-4")[1].textContent = "iNeuron";
document.getElementsByClassName("color-base-70 mb-4")[1].innerText = "I Write Code";
```
<hr>

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

## Answer
```
let output = [];

for (let i=0; i<document.getElementsByClassName("as-imagegrid-item-title").length; i++){
    output.push(document.getElementsByClassName("as-imagegrid-item-title")[i].firstChild.data);
}

console.log(output);
```
<hr>

3. Website Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

## Answer
```
let new_section = document.createElement("section");
new_section.className = "parent";

let new_faq = document.createElement("h3");
new_faq.innerText = "My New FAQ";

new_section.appendChild(new_faq);

let topics = document.querySelector(".accordion-homepage");
topics.appendChild(new_section)

```
<hr>

4. Website Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

## Answer
```
document.getElementsByClassName("one-tel-number service-number")[0].textContent = "+91 6366256689"

```
<hr>

5. Website Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)

## Answer
```
for (let i=0; i<document.querySelectorAll(".diwali-deals-product-sale-btn").length; i++){
    document.querySelectorAll(".diwali-deals-product-sale-btn")[i].innerText = "Check out";
}

```
<hr>

6. Website Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)

## Answer
```
let search = document.getElementsByClassName("searchinput___19uW0")[0]

function colorRed() {
    search.style.backgroundColor = "Red";
}

search.addEventListener("mouseover", colorRed);

```
<hr>

7. Website Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

## Answer
```
document.getElementById("top-nav-search-input").setAttribute("value", "hi" );
document.getElementsByClassName("button action has-icon search-button")[0].click()
```
<hr>

8. Website Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

## Answer
```

```
<hr>

9. Website Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

## Answer
```
document.getElementsByClassName("display-heading-1")[0].style.fontFamily = "monospace"

document.getElementsByClassName("display-heading-1")[0].style.color = "Red"

```
<hr>

10. Website Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

## Answer
```
const button = document.getElementsByClassName("login-btn-text")[1];

const changeColor = () =>{
    button.style.backgroundColor = "Red";
}

button.addEventListener("mouseover", changeColor);

```
<hr>

11. Website Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

## Answer
```
document.getElementsByClassName("icon icon-logo in")[0].style.backgroundImage = "url('https://account.ineuron.ai/static/images/ineuron-logo.png')";

```
<hr>

12. Website Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

## Answer
```
document.getElementsByClassName("btn btn-sm btn-primary")[0].style.backgroundColor = "blue";

```
<hr>

13. Website Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

## Answer
```
document.getElementsByClassName("fl-heading-text")[0].innerText = "JS Bootcamp"

```
<hr>

14. Website Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

## Answer
```
document.getElementsByClassName("HotDealsAll__Heading__2fIbe")[0].style.fontSize = "80px"
```
<hr>

15. Website Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

## Answer
```

```
<hr>

16. Website Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)

## Answer
```
document.getElementsByClassName("section-title_title__VEDfK")[0].innerHTML = "Start with Scratch"
```
<hr>

17. Website Name: [Sony](https://www.sony.co.in/electronics/televisions/x90k-x93k-x94k-series?cpint=homepage_whats_hot-What%27s%20Hot-en_IN-responsivegrid_structure_top_whtshot_1)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)

## Answer
```
const button = document.getElementsByClassName("btn btn-large btn-block buy buy-button retailer_btn-align")[0]

button.innerHTML = new Date()
```
<hr>

18. Website Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

## Answer
```
document.getElementsByClassName("p-f03-footer-container ")[0].style.background = "none";
document.getElementsByClassName("p-f03-footer-container ")[0].style.backgroundColor = "orange"
```
<hr>

19. Website Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

## Answer
```
document.getElementsByClassName("logo")[0].getAttribute("src")
```
<hr>

20. Website Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

## Answer
```
const desc = document.getElementsByClassName("desc")

for (let i=0; i<desc.length; i++){
    desc[i].style.color = "orange";
}
```
<hr>