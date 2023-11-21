---
layout: posts
title: Triange
---

![alt text](../assets/images/triangle.png "triangle")
<html>
    <head>
        <title>triangle</title>
    </head>
    <body>
        
        <h1 style="text-align: center;font-family:tahoma">Tringle</h1>
        
            <div style="font-size:larger;" dir="ltl">
               <pre>
import turtle
import random

def triangle(d):
    if d<5:
        return 
    turtle.fillcolor(random.random(),random.random(),random.random())
    turtle.begin_fill()
    for _ in range(3):
      triangle(d/2)
      turtle.forward(d)
      turtle.left(120)
    turtle.end_fill()
turtle.tracer(0)
triangle(300)      
turtle.update()
turtle.mainloop()</pre>
                
   
               <a href="file:///C:/git/FC02031/S9/django1/tree.html">
                Tree
           </a> 
      
            </div>
            
        
       
    </body>
    </html>