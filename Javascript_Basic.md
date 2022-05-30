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

#### document.write("")>> display text to html (for this lesson)
```
document.write("<h1> HAHAHA THIS IS OTHER FILE </h1>");
document.write("<p>LOREN IPSUM SADJKSADIJGFIARJNGKAIJGAORN </p>")
```

#### alert("") is popup
```
alert("Yay Popup!");
alert("");
```
#### console.log("") is debug'text in console
```
console.log("You can find me in console :3");
```
#### console.error("") is error in console (red)
```
console.error("just error");
```
#### console.error("") is warning in console (yellow)
```
console.warn("just warning");
```
#### // << is comment
#### /* << is open comment | is end of comment */

#### Rule of variable >> name+num / no special syntax no num / can $ and _ / can case sensitive / no keyword (if else etc.)
- Dynamic Typing > free variable
- Static Typing > with variable

#### Example 'var' (var = old tpye)
```
var money;
money=200;
var a,b,c,d;
var x=20, y=30;
```
> if undefind no type of variable 
#### Example 'let' (let = new version)
- let can modify number
```
let same, Same=200, ans;
same = 300; 
ans = same-Same;
document.write(ans);
```
- const is lock value cannot modify and require number
```
const dam=100;
document.write(dam);
dam = same+Same;
document.write(dam);
```
#### DATA TYPE
##### NUM INTEGER  : 20
```
let nnn=20;
console.log(nnn);
console.log(typeof(nnn));
```
##### NUM FLOAT    : 20.15
```
let mmm=20.15;
console.log(mmm);
console.log(typeof(mmm));
```
##### STRING       : "TEXTSTRING" || 'TEXTSTRING'
```
let ttt="TEXTSTRING";
let TTT='TEXTSTRING';
let TtT="20";
```
##### BOOLEAN      : TRUE|FALSE (True=1 False=0)
```
let FLS=false;
console.log(FLS);
let TRU=true;
console.log(TRU);
```
##### OBJECT       : {data:"string",age:"number"}
##### ARRAY        : ["APPLE","PINEAPPLE","APPLEPINE"]
##### TYPEOF : CHECK DATA TYPE
##### NULL : NO DATA | DATA is NULL
##### UNDEFINED : no value/data in variable

#### Change STRING to NUMBER
##### if
```
let a="20";
console.log(a);
console.log(a+20);
console.log(typeof(a));
let b="20.20";
console.log(b);
console.log(b+20);
console.log(typeof(b));
```
##### Result
```
20
2020
String
20.20
20.2020
String
```
##### How to Change
- INTIGER
```
a = parseInt('a');
```
- FLOAT
``` 
b = parsaFloat('b');
```
##### Change INT to STRING
```
a.toString();
""+a
```
