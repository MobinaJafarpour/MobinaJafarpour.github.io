---
layout: posts
title: Jungle
---

![alt text](../assets/images/JUNGLE.png "jungle")

<html>
    <head>
        <title>jungle</title>
    </head>
    <body>
        
        <h1 style="text-align: center;font-family:tahoma">Jungle</h1>
        
            <div style="font-weight: bold;font-size:larger;" dir="ltl">
               <pre>
                import turtle
                import random
                
                def Tree(d,a,w):
                    if d < 5 or a < 5:
                        return turtle.dot(13,"pink")
                    
                    turtle.pendown()
                    turtle.pensize(w)
                    turtle.forward(d)
                    turtle.left(a)
                    Tree(d * (random.random()/2 + 0.5), 
                         a * (random.random()/2 + 0.7), 
                         w * (random.random()/2 + 0.5))
                    turtle.right(2 * a)
                    Tree(d * (random.random()/2 + 0.5), 
                         a * (random.random()/2 + 0.7), 
                         w * (random.random()/2 + 0.5))
                    turtle.left(a)
                    turtle.backward(d)
                
                
                width, height = 1800, 1000
                x=-width/2 + 100
                y=-height/2
                
                tree_count = 20
                
                turtle.tracer(0)
                turtle.left(90)
                
                for ـ in range(tree_count):
                    x = random.randint(-500, 500)
                    y = random.randint(-350, -200)
                    turtle.penup()
                    turtle.setpos(x, y)
                    turtle.pendown()
                    Tree(
                        random.randint(25, 100), 
                        random.randint(5, 20), 
                        random.randint(5, 15))
                
                
                turtle.update()
                
                turtle.mainloop()

                
                
                <a href="file:///C:/git/FC02031/S9/django1/triangle.html">
                     Triangle
                </a> 

            </div>
            
        
       
    </body>
    </html>