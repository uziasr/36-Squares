# 36-Squares
# Using loops, I will create multiple squares 
import turtle

window = turtle.Screen()
window.bgcolor("blue")
brad = turtle.Turtle()
brad.shape("turtle")
brad.color("yellow")
brad.speed(5)
def draw_u(x):
    for i in range (1,4):
        x.left(90)
        x.backward(100)
#brad will replace the x value when draw_square is used        
def draw_square (x):
    for i in range (1,5):
        x.forward(100)
        x.right(90)
def draw_circle (y):
    y.circle(100)
    
def draw_art():

    for i in range (1,37):
#here brad will go through the draw_square function
#and use forward and right to make square
       draw_square(brad)
       brad.right(10)
    #draw_circle(brad)
    #draw_u(brad)
    window.exitonclick()

draw_art()
