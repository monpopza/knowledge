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
- change from (many variable)
```
let num1 = 1; num2 = 2; num3 = 3;
console.log(num1,num2,num3)
```
> result
```
123
```
- to one variable
```
let num = Array(1,2,3);
console.log(num);
```
> result
```
(3) [1, 2, 3]
0. 1
1. 2
2. 3
```
- how to use array
```
if i want to use 3 
console.log(num[2])
of i want to use 1
console.log(num[0])
```
if string 
```
let color = Array("red","blue","yellow","white");
console.log(color);
```
> result
```
(4) [red,blue,yellow,white]
0. red
1. blue
2. yellow
3. white
```
> hot to change value in array[]
```
color[0] = "green";
```
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
- String to INTIGER
```
a = parseInt('a');
```
- String to FLOAT
``` 
b = parsaFloat('b');
```
##### Change int/float to STRING
```
a.toString();
a+""
```

## Operator abd operand
### Caculator
``` + - * / % ** ```
> % = ผลเศษ
> ** = squar
```
console.log(1+1);
console.log(1*1);
console.log(1/1);
console.log(1-1);
console.log(1%1);
console.log(2**1);
```
### Boolean
``` == != > < >= <= ```
- how to use
```
let a = Array(1,2,3)l
console.log(a[1]==a[2]);
console.log(a[1]!=a[2]);
console.log(a[1]>a[2]);
console.log(a[1]<a[2]);
console.log(a[1]>=a[2]);
console.log(a[1]<=a[2]);
let t=true;
console.log(!true);
```
> Result
```
false
true
false
true
false
true
false
```
- and or not
```
and = &&
or = ||
not = !
```
- how to use
```

```
### Add ans Redude Value
```
let a = 0;
console.log(a);  
console.log(a++); << Postfix
console.log(a); 
console.log("-------"); 
a = 0;
console.log(a); 
console.log(++a); << Prefix
console.log(a); 
console.log("-------"); 
a = 0;
console.log(a); 
console.log(a--);  << Postfix
console.log(a); 
console.log("-------"); 
a = 0;
console.log(a); 
console.log(--a);  << Postfix
console.log(a); 
console.log("-------"); 
```
> Result
```
0 
0  << Postfix เพิ่มนะแต่ไม่แสดง
1
-------
0
1  << Prefix เพิ่มและแสดงออกมาเลย
1
-------
0
0  << Postfix
-1
-------
0
-1  << Postfix
-1
-------
```
## Conpound Assignment
```
_______________________
| += | x+=y | x = x+y |
| -= | x-=y | x = x-y |
| *= | x*=y | x = x*y |
| /= | x/=y | x = x/y |
| %= | x%=y | x = x%y |
_______________________
```
## Priority Calculate
``` 
__________________________
| 1 |    ( )    |   -    |
| 2 |   ++  --  | L to R |
| 3 |   * / %.  | L to R |
| 4 |    + -    | L to R |
| 5 | < <= > >= | L to R |
| 6 |   == !=   | L to R |
| 7 |     &&    | L to R |
| 8 |     ||    | L to R |
| 9 |  = += -=  | R to L |
|   | *= /= %=  |        |
__________________________
```
## IF Statement
- Sequence
 - if
```
if (quesion-true) {
    whatever you want to do;
}
else{
whatever you want to do other;
}
```
> if else แบบย่อ
```
let ans = quesion-true ? whatever you want to do:whatever you want to do other;
|       |    Quesion     |         IF           |            ELSE             |
console.log(ans);
```
 - if  ไปเรื่อยๆถ้าไม่ได้ก็ไม่มี ผล if
```
if(){
}if(){
}
```
 - if ซ้อน if
```
if(quesion1-big){
    if(quesion2-small){
    aa
    }else if(quesion3-small){
    bb
    }else (quesion4-small){
    cc
    }
}else{
not match;
}
```
 - Example 
```
let a = 10;
if (a>=10)}
    console.log("You in 10");
}else{
    console.log("you not in 10 Please check your device");
}
<--------------------------------------------------------->

```
 - Switch..Case
 > same if but one way only
```
switch(quesion-check){
    case value1:do1; 
    break;
    case value2:do2;
    break
    ...
    case valueN:doN ;
    defalut:dodefalutl
}
```
- Condition
```
```
- Loop
```break,continue```
 - break
Stop and skip to outloop!
```
for(let i;i<=10:i++){
    if(i==5)break;
    condsole.log
}
console.log("END");
```
> stop at 4 and stop
 - continue
Stop and Renew same loop
```
for(let i;i<=10:i++){
    if(i==5)continue;
    condsole.log
}
console.log("END");
```
> skip at 5 and continue

```while,For,Do..While```
 - While
```
let a=0;
while(a<=5){
    do somthing;
    if(a==4){break;}
    a++;
}

```
 - For loop 
```
for(let i=1;i<=10;i++){
    True
}
```
 - Do..While
ทำรอบนึงแล้วเชค
```
let i=0;
do{
    console.log(i);
    i++;
}while(i<=5);
```
