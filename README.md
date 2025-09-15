# Moon-Rising
#python code idk
import turtle as trtl
painter = trtl.Turtle()
water = trtl.Turtle()
import random


painter.hideturtle()
painter.penup()
painter.goto(0,-600)
painter.pencolor()
painter.pendown()
painter.begin_fill()
painter.speed(0)
painter.circle(750)
painter.fillcolor()
painter.end_fill()
painter.showturtle()
painter.goto(0,0)
painter.shape("circle")
painter.color("yellow")
painter.turtlesize(0.25)
painter.penup()
stars = 0


while (stars <= 50):
    starx = random.randint( -500, 400 )
    stary = random. randint (-300, 400)
    painter.hideturtle()
    painter.goto(starx,stary)
    painter.pendown()
    painter.showturtle()
    painter.clone()
    painter.penup()
    painter.goto(0,0)
    stars = stars + 1


water.speed(0)
water.goto(-550,-300)
water.pendown()
water.color("midnightblue")
water.begin_fill()
water.forward(2000)
water.right(90)
water.forward(200)
water.right(90)
water.forward(2000)
water.right(90)
water.forward(200)
water.fillcolor("midnightblue")
water.end_fill()
water.penup()


painter.hideturtle()
painter.left(45)
painter.turtlesize(10)
painter.goto(-800,-200)
painter.speed(1)
painter.color("LightGoldenRod")
painter.shape("circle")
painter.showturtle()
painter.forward(700)
painter.stamp()


wn = trtl.Screen()
wn.mainloop()






