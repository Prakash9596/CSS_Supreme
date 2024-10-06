# CSS Supreme

--> Comment in HTML: <!-- Comment -->
--> Comment in CSS:  /* Comment */

--> Priority: ( Inline Styling > Internal Styling > External Styling )
--> Priority: ( Element/ID/Class/Group/Descendant selector > Universal selector )

--> Search Colour picker: To get the code of any colour.
--> Background Shorthand can be defined as (color, image, repeat, attachment, position)
    background: green url('jeans.webp') no-repeat center;

--> font-weight can be between (100 to 900) (Normal=400, Bold=700)
--> font-family can be download from google fonts. (Copy link put it in head and copy font-family put it in style)
--> Icons can be downloaded from https://fontawesome.com (Copy script put it in head and copy <i></i> put it in body)

--> CPBM Model(Content Padding Border Margin)
--> padding: 5px 10px 15px 20px; (Top Right Bottom Left): C.W
    padding: 5px; means its the same for all four sides.
    padding: 5px 10px; means (top and bottom =5px) & (Right and lefy =10px)

--> margin: 15px 10px 25px 20px; (Top Right Bottom Left): C.W
    Margin between 2 boxes will be the one which is greater. 
    ex:(box1: bottom margin=10px, box2: top margin=20px), then margin between both the boxes=20px

--> border: 2px solid red; (border: weight type colour)
    border-radius: 5px 15px 5px 5px; (Top-left Top-right Bottom-right Bottom-left)

--> Element size=content + padding + border, Note: margin will not be counted in element size
--> Div ka height: 50px; width: 50px;
      box-sizing: content-box; (57.2 * 57.2) = 50(height/width)+{2+2}(padding)+{1.6+1.6}(border), 
      ye by-default hota h (border 2px= 1.6 me badal gya thoda km ho jata h)
         
      box-sizing: border-box; (50 * 50) = 42.8(height/width)+{2+2}(padding)+{1.6+1.6}(border), 
      (height, width, padding and border usi me aayega)

--> Browser sources will contain all the sources which is required for that page.
--> Browser network will show from where it downloaded all the required files.
--> Browser performance will show the performance of the page.
--> Browser console shows the output.
--> Browser elements shows the code.
--> Browser application shows different types of storage.
--> Broswer memory shows memory details i.e heap memory, run time memory, memory allocation. 

--> visibility: hidden; Visibility hidden hai phir bhi apna space to lega ye bs apne ko dikh nhi rha bs.

--> display: block; By-default hota hai jiska mtlb ye naye line se shuru hoga as its a block element.
--> display: inline; hone ke wajah se div ab ek line me aa rha hai but size jo hm 100px*100px set kiye hain wo pick nhi kr rha h why ?
    becoz its inline element now and its Styling is Limited: Can't set size easily. 
    Iska size content ke size ke according hoga, irrespective ki aap koi height and width de rhe hain.
    Iska solution hai display: inline-block;
--> display: inline-block; This is the solution of display_inline.
--> display: none; visibility: hidden;
    display: none; Isse invisible to hoga hi hoga saath hi saath apna height aur width v leke chala jayega.
    visibility: hidden; Isse invisible to hoga pr height aur width rhega.

--> Responsive Website:
Relative Units:
1. px: Static unit in pexels
2. %: It is relative to its parent. (If parent is not there then it will treat page size as parent size) 
      Ex: width: 50%; (50% of its parent)
3. em: Ex: font-size: 2.5em (2.5 times of its parent)
4. rem: Ex: font-size: 2rem; (2 times of its root parent)
   Note: em & rem are only for font size.
5. vh: viewport height, Ex: height: 50vh; (50% of page)
6. vw: viewport width, Ex: width: 90vw;(90% of page) 
        
-->Position Property:
• Static (default) : Its static.
• Relative: Element's relative position from its normal position.
• Absolute: Element's relative position from page or its nearest positioned ancestor. (ek ke upar ek chadh jate hain)
• Fixed: Element's relative position from viewport(Page), does not move on scroll. (ek ke upar ek chadh jate hain)

--> z-index: mtlb z-axis pe ek ke upar ek, jiska z-index jitna jyda hoga wo utna upar hoga.
    Ex: z-index: 2; (2nd level pe hoga)

--> Flexbox: It is a one-dimensional layout method for arranging items in rows or columns.
    Flex Items(expand) to fill additional space or shrink to fit into smaller spaces.
    Flex container >> Flex Items --> Main axis: Left to right, Cross Axis: Top to bottom
--> ye sara property flex container pe lag rha hai.
     flex-direction:row; Left to right (main axis ke along)
     flex-direction:row-reverse; Right to Left (main axis ke along)
     flex-direction:column; Top to bottom (main axis ke along)
     flex-direction:column-reverse; Bottom to top (main axis ke along)

--> ye sara property flex container pe lag rha hai.
    Flex Justify Content: tb use hota hai jb hmara box container ke size se chhota hota hai. (main axis ke along)
    Flex wrap: isse box apna size chhota nhi krega wo pure container ke andar wrap ho jayega. (main axis ke along)
    Flex align items: isse box ko hm cross axis ke along adjust kr skte hain. (cross axis)
    Flex align Content: Isse cross axis me box ke bich ka space manage kiya jata hai. (cross axis)

--> ye sara property flex items pe lag rha hai flex container pe nhi.
    Flex align self: isse kisi particular flex item ka cross axis me position change kr skte hain.
    Flex Shrink/Grow: Isse kisi particular flex item ko shrink/ grow krwa skte hain ..jb flex wrap property use na ho rha ho.
    wrna flex wrap krenge to flex iteam shrink/grow hoga hi nhi na.

--> Flex Items (Order)
The "order" property in CSS allows you to define the sequence in which flex items appear within the flex
container, overriding their original order in the HTML.  This is also flex item propety.

--> GRID: 2D layout system for rows & columns. Individual units called grid cells.

--> @media screen and (width: 800px) {
            .box { border: 5px solid red; background-color: aqua; }
        }
    @media screen and (min-width: 250px) and (max-width: 700px) {
            .box { border-radius: 50%; }
        }

--> transition-property: all; transition-duration: 1s; transition-timing-function: ease-in-out/steps(3); transition-delay: 0.2s;
--> transition: all 1s ease-in-out 0.2s; [Shorthand] 

    transition-property: all; (jo-jo property iske liye defined h sb use kro)
    transition-duration: 1s; (Ye 1sec me complete ho jana chahiye)
    transition-timing-function: ease-in-out/steps(3); (hone ka tarika kya hoga)
    transition-delay: 0.2s; (starting delay kitna hoga)

--> animation-name: ghumakkad; animation-duration: 4s; animation-timing-function: ease-in-out;
    animation-delay: 0s; animation-iteration-count: 4; animation-direction: normal/alternate/reverse/alternate-reverse;
--> animation: ghumakkad 4s ease-in-out 0s 4 alternate; [Shorthand] 
    
    animation-name: ghumakkad; (naam rakh do kuchh bhi)
    animation-duration: 4s; (kitna der me animation complete hoga)
    animation-timing-function: ease-in-out; (kis tarah se animate krega)
    animation-delay: 0s; (starting delay kitna hoga)
    animation-iteration-count: 4; (total kitna baar same chij hoga)
    animation-direction: normal/alternate/reverse/alternate-reverse; (direction kya hoga)

    @keyframes ghumakkad { from {left: 10px}  to {left: 300px} }
    @keyframes ghumakkad { 0%{left: 10px; top: 0px} 50%{ left: 150px; top: 100px } 100%{left: 300px; top: 0px} }



--> Quick Recall:
1.  h1 { color: green; } & p { color: red;} --> Colour property
2.  <h1 style="color: red;">Inline Styling</h1> --> Inline styling
3.  <style> h1{color: green;} p{color: red;} </style> --> Internal styling (head ke andar)
4.  <link rel="stylesheet" href="/Course Code/css/level 1/4.external styling.css"> --> External styling (head ke andar)
5.  h1 {color: red;} --> Element selector
6.  * {color: red;} --> Universal selector
7.  <div id="first">First Div</div> & #first{ color: red;} --> ID selector
8.  <div class="second">Second Div</div> & .second { color: green; } --> Class selector
9.  h1, h2, h3 {color: red;} --> Group selector
10. #first p { color: red;} --> Descendant selector
11. #first {background-color: green;} --> Background Color property
12. <div style="background-color: rgb(0,255,0);">Second</div> --> RGB Model
13. <div style="background-color: #0000ff;">Third</div> --> hex model
14. <h1 style="color: rgba(255,0,0,0.5);">First</div> --> aplha/rgba model (To set transparency)
15. .box {height: 40px; width: 40px;} --> To set height and width
16. background-color: green;
    background-image: url(../../images/OIP.jfif); --> To set Background Image
    background-repeat: no-repeat; --> Image apne bnaye div me repeat krega ya nhi.
    background-position: right; --> Image apne bnaye div me kis position pe hoga
    background-size: contain; --> Image div se bada ho ya chhota apne div me adjust kr lega
    --> background: green url('jeans.webp') no-repeat center;
17. #box1 {visibility: hidden;} --> hide ho jayega pr space lega page ke upar
    #box2 {visibility: visible;} --> by-default yhi hota h 
18. #box1 {text-align: center/left/right;} --> box1 ke andar text ka alignment kaisa hoga
19. #box1 {text-decoration: underline/overline/line-through;} --> text underlined/overlined/line-through kaisa hoga
20. #box1 {text-decoration-style: dashed/double/solid/wavy;} --> text underline krne ka alag alag tarika
21. #box1 {text-decoration-color: red;} --> text decoration kis colour se hoga
22. #box1 {text-transform: uppercase/lowercase/capitalize/none;} --> text ko transform krne ka tarika
23. #first { line-height: 6px; } --> lines ke bich kitna gap hoga
24. #first {font-size: 5px;} --> font-size kya hoga
25. #third {font-weight: 600;} --> font weight kya hoga mtlb boldness of font
26. #first {font-style: italic/oblique/normal;} --> font likhne ka tarika
27. #first {font-family: Arial, Helvetica, sans-serif;} --> font family de rhe for fallback mechanism
    font-family can be download from google fonts. (Copy link put it in head and copy font-family put it in style)
28. <i class="fa-brands fa-tiktok"></i> --> icons bnane ke liye
    Icons can be downloaded from https://fontawesome.com (Copy script put it in head and copy <i></i> put it in body)
29. padding: 5px 10px 15px 20px; /*(Top Right Bottom Left): C.W*/
    padding: 5px; means its the same for all four sides.
    padding: 5px 10px; means (top and bottom 5px) & (Right and lefy 10px)
30. margin: 15px 10px 25px 20px; /*(Top Right Bottom Left): C.W*/
31. border: 3px dotted/solid red;
32. border-radius: 5px 15px 5px 5px; /*(Top-left Top-right Bottom-right Bottom-left)*/
33. box-sizing: content-box; (Div ka height: 50px; width: 50px; --> content-box: (57.2 * 57.2))
    box-sizing: border-box; (Div ka height: 50px; width: 50px; --> border-box: (50 * 50))
34. display: block;  By-default hota hai jiska mtlb ye naye line se shuru hoga as its a block element.
    display: inline; ke wajah se div ab ek line me aa jayega hai but size jo hm 100px * 100px set kiye hain wo pick nhi krega.
    display: inline-block; This is the solution of display_inline.
    display: none; Isse invisible to hoga hi hoga saath hi saath apna height aur width v leke chala jayega.
35. width: 50%; height: 30%;  It is relative to its parent. To make Website Responsive.
    font-size: 2em; /* Twice of my parent i.e 50px */
    font-size: 2rem; /* mtlb 2 times of root parent */
    height: 50vh; width: 90vw; /* 50% & 90% of viewport i.e. page*/
36. position: static; Its static.
    position: relative;top: 20px;left: 90px; Element's relative position from its normal position.
    position: absolute;top: 200px;left: 150px; Element's relative position from page or its nearest positioned ancestor. (ek ke upar ek chadh jate hain)
    position: fixed;top: 20px;left: 65px; Element's relative position from viewport(Page), does not move on scroll. (ek ke upar ek chadh jate hain)
37. z-index: 2; z-index: mtlb z-axis pe ek ke upar ek, jiska z-index jitna jyda hoga wo utna upar hoga.
38. float: right/left; iska use krke hm kisi container me box ko display kra skte hain righmost/leftmost me.
39. display: flex; Jisse block/div flex bn jayega
    flex-direction: row/row-reverse/column/column-reverse; and ush flex ka direction aise decide hoga. (along main axis)
40. display: flex;
    justify-content: flex-start/flex-end/Center/space-between/space-around/space-evenly; (along main axis)
41. display: flex;
    flex-wrap: wrap/wrap-reverse; (along main axis)
42. display: flex;
    align-items: center/start/end; isse box ko hm cross axis ke along adjust kr skte hain.
43. display: flex;
    align-content: center/start/end; Isse cross axis me box ke bich ka space manage kiya jata hai.
44. display: flex; [ye display:flex container pe lgta hai jbki align-self flex item pe lgta h]
    align-self: center/start/end; isse kisi particular flex item ka cross axis me position change kr skte hain.
45. flex-shrink: 1; normally sbke jaisa shrink hoga
    flex-shrink: 0.5; sb jitna shrink ho rha h usse aadha hoga.
    flex-shrink: 0; ye to shrink hoga hi nhi.
    flex-grow: 1; jitna space h uske according.
    flex-grow: 4; sb jitna grow ho rha h usse 4 times jyada hoga.
46. display: flex; flex container pe aayega
    order: 3; flex items pe aayega
47. .container {display: grid; grid-template-columns: 50px 50px; grid-template-rows: 50px 50px;}
    .item1 {grid-column: 1 / 2; grid-row: 1 / 2;}
48. @media screen and (width: 800px) {
            .box { border: 5px solid red; background-color: aqua; }
        }
49. @media screen and (min-width: 800px) {
            .box { height: 150px; width: 150px; }
        } --> (min-width: 800px) mtlb (800 ya 800 se jyada) --> (max-width: 800px) mtlb (800 ya 800 se km)
50. @media screen and (min-width: 250px) and (max-width: 700px) {
            .box { border-radius: 50%; }
        }
51. .btn { height: 20px; width: 70px; background-color: lightcoral; }
    .btn:hover { height: 25px; width: 80px; background-color: red;}
    .btn:active { height: 25px; width: 80px; background-color: rgb(92, 205, 147); }
52. .btn { height: 20px; width: 70px; background-color: lightcoral;
           transition-property: all; transition-duration: 1s; transition-timing-function: ease-in-out/steps(3); transition-delay: 0.2s;}
           ----->>> transition: all 1s ease-in-out 0.2s;
    .btn:hover { height: 25px; width: 80px; background-color: red;}
    .btn:active { height: 25px; width: 80px; background-color: rgb(92, 205, 147); }
53. .btn { height: 20px; width: 70px; background-color: lightcoral; transition: all 1s ease-in-out 0.1s;}
    #btn1:hover { transform: rotate(45deg); }
    #btn2:hover { transform: rotate(180deg); }
    #btn3:hover { transform: rotatex(45deg); }
    #btn4:hover { transform: rotatey(45deg); }
    #btn5:hover { transform: rotatez(45deg); }
54. .btn { height: 20px; width: 70px; background-color: lightcoral; transition: all 1s ease-in-out 0.1s;}
    #btn1:hover { transform: scale(2); }
    #btn2:hover { transform: scale(4); }
    #btn3:hover { transform: scalex(2); }
    #btn4:hover { transform: scaley(3); }
    #btn5:hover { transform: scaleZ(2) }
55. .btn { height: 20px; width: 70px; background-color: lightcoral; transition: all 1s ease-in-out 0.1s;}
    #btn1:hover { transform: translate(50px); }
    #btn2:hover { transform: translate(50px, 50px); }
    #btn3:hover { transform: translatex(50px); }
    #btn4:hover { transform: translatey(50px); }
56. .btn { height: 20px; width: 70px; background-color: lightcoral; transition: all 1s ease-in-out 0.1s;}
    #btn1:hover { transform: skew(45deg); }
    #btn2:hover { transform: skew(90deg); }
57. .box { height: 75px; width: 75px; background-color: lime;
           animation-name: ghumakkad; animation-duration: 4s; animation-timing-function: ease-in-out;
           animation-delay: 0s; animation-iteration-count: 4; animation-direction: normal/alternate/reverse/alternate-reverse;}
           ----->animation: ghumakkad 4s ease-in-out 0s 4 alternate;
    @keyframes ghumakkad { from {left: 10px}  to {left: 300px} }  (Left se right ki taraf animate krega)
58. .box { height: 75px; width: 75px; background-color: lime;
           animation-name: ghumakkad; animation-duration: 4s; animation-timing-function: ease-in-out;
           animation-delay: 0s; animation-iteration-count: 4; animation-direction: normal/alternate/reverse/alternate-reverse;}
           ----->animation: ghumakkad 4s ease-in-out 0s 4 alternate;
    @keyframes ghumakkad { 0%{left: 10px; top: 0px} 50%{ left: 150px; top: 100px } 100%{left: 300px; top: 0px} }


