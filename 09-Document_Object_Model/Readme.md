Document Object Model, every HTML page translated into the DOM so that it can be
parseable by the JavaScript. Check the description in Part1_MainPage.html

```JavaScript
document.getElementById("sampleid")
<li id=​"sampleid">​::marker​"document.URL -- This is the actual URL of the website"</li>​
document.getElementsByClassName("myul")
HTMLCollection(2) [ul.myul, ul.myul]0: ul.myulaccessKey: ...

document.getElementsByTagName("li")
HTMLCollection(9) [li#sampleid, li, li, li, li, li, li, li, li, sampleid:

The query selector works in other way similar like selecting the CSS tag
document.querySelector("#sampleid")
<li id=​"sampleid">​…​</li>​  

document.querySelectorAll(".myul") // Using the .myul here same as CSS selector
NodeList(2) [ul.myul, ul.myul]
```
The main intention of this DOM is to grab an element and then change the property of that element so that the user can see it how we want to show it. The example is the Part1_Color_Changer.js script

```JavaScript
// Grab
var header = document.querySelector("h1")
// set
header.style.color = 'red'
```

How to change the content inside the HTML

```JavaScript
var p = document.querySelector("p")
undefined
p
<p>​"To Edit Styles, we've already seen we can use the .style tag. Now if we want to edit "<strong>​actual html or text​</strong>​" or "<a href=​"http:​/​/​www.google.com">​attributes​</a>​" we can use different methods. If you want to change the text,html content, or attributes you can use the following: "</p>​
p.textContent = "new text"
'new text'
// But we can't make it bold
undefined
// use instead this
undefined
p.innerHTML = "<strong>I'm bold</strong>"
"<strong>I'm bold</strong>"
