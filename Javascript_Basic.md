# JavaScript Basic 
## Source 
- Lacture : https://www.youtube.com/watch?v=AbjY-ajKgSI&t=2931 (TH)
## File (.html) 
### index.HTML 
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8"/>
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <title>JS Basic</title>
        <!-- Internal JS use one oly file >> script type="text/javascript">
            document.write("<i>n4mmon.com</i>");
        </script -->
       <!-- External JS can use multifile -->
        <script src="./app.js"></script>
    </head>
    <body>
    </body>
</html>
```
## File Javascript (.js)
### App.js
```
// document.write("")>> display text to html (for this lesson)
document.write("<h1> HAHAHA THIS IS OTHER FILE </h1>");
document.write("<p>LOREN IPSUM SADJKSADIJGFIARJNGKAIJGAORN </p>")

// alert("") is popup
//alert("Yay Popup!");
//alert("");

//console.log("") is debug'text in console
//console.log("You can find me in console :3");

//console.error("") is error in console (red)
//console.error("just error");

//console.error("") is warning in console (yellow)
//console.warn("just warning");

// << is comment
/* << is open comment | is end of comment */

/* ---------------------------------------------------------------------------------- */
// Rule of variable >> name+num / no special syntax no num / can $ and _ / can case sensitive / no keyword (if else etc.)
// Dynamic Typing > free variable
// Static Typing > with variable

// Example 'var' is money (var = old tpye)
var money;
money=200;
var a,b,c,d;
var x=20, y=30;

// if undefind no type of variable
// Example 'let' is katy (let = new version)
// let can modify number
let same, Same=200, ans;
same = 300; 
same - Same == ans;
document.write(ans);
// const is lock value cannot modify and require number
const dam=100;
```
