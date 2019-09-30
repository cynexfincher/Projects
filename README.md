import turtle   # The following program needs a library named turtle
import math     # The following program needs a library named math
 


'''THE FOLLOWING CODE IS FOR MAKING THE BACKGROUND'''

t1 = turtle.Turtle()
t1.hideturtle() # There is a turtle named t1. It is used for drawing the background  
def draw_circle():    # This function uses the concept of concentric circles with a difference of the radius being 100 and 50.
  # This was done with the help of Rahul K (skakar3@uic.edu)
 t1.color("black")
 t1.dot(1000)
 t1.color("darkred") 
 t1.dot(500)
 t1.color("chocolate")
 t1.dot(400)
 t1.color("darkorange") 
 t1.dot(300)
 t1.color("gold") 
 t1.dot(200)
 t1.color("lemon chiffon") 
 t1.dot(100)
 t1.color("white") 
 t1.dot(50)
 


'''THE FOLLOWING CODE IS MEANT TO DRAW THE TREE'''

t2 = turtle.Turtle() # There is a turtle named t2. It is used for drawing the tree. The tree uses the concept of fractionals.
t2.shape("arrow")    # The turtle is given a different shape so that the process can be differenciated
t2.lt(90)
t2.hideturtle()

lv = 11
l  = 50
s  = 17


def draw_tree(l, level): # This function is the example of the concept of looping with 'if' conditions. It uses the turtle t2.
    t2.speed(100)
    t2.pendown()
    l = 7.0/8.0*l
    t2.lt(s)
    t2.fd(l)
    level +=1
    if level<lv:
        draw_tree(l, level)

    t2.bk(l)
    t2.rt(2*s)
    t2.fd(l)
    if level<=lv:
        draw_tree(l, level)
    t2.bk(l)
    t2.lt(s)
    level -=1

t2.speed(100)        



'''THE FOLLOWING CODE IS MEANT FOR DRAWING THE GROUND'''
  
t3 = turtle.Turtle() # There is a turtle named t3. It is meant for drawing the ground. The ground uses a 'for' loop. 

def ground(): # The following function is being defined to draw the ground using the turtle t3.
 t3.speed(100)
 t3.pensize(3)
 t3.setpos(500, 0)
 t3.rt(90)
 g = 1000
 t3.rt(90)
 for i in range (20):
    t3.fd( g )
    
    t3.rt(181)
    g = g - 20
    t3.fd ( g )
    t3.rt (179)
    g = g - 20

'''THE FOLLOWING CODE IS MEANT FOR DRAWING A HOUSE'''

t4 =  turtle.Turtle() # There is a turtle called t4. This is being used for drawing the house. 
def draw_polygon(): # The following function being defined is meant for drawing the house.
 t4.speed(10)
 t4.hideturtle()
 t4.penup()
 t4.setpos(250,100)
 t4.rt(90)
 t4.fd(100)
 t4.begin_fill()
 t4.pendown()
 t4.rt(90)
 t4.fd(100)
 t4.rt(90)
 t4.fd(150)
 t4.rt(45)
 t4.fd(150)
 t4.rt(90)
 t4.fd(150)
 t4.rt(45)
 t4.fd(150)
 t4.rt(90)
 t4.fd(100)
 t4.rt(90)
 t4.fd(40)
 t4.lt(90)
 t4.fd(20)
 t4.lt(90)
 t4.fd(40)
 t4.lt(90)
 t4.fd(30)
 t4.end_fill()
 t4.color("red") # Changing colours for the window.
 t4.penup()
 t4.lt(90)
 t4.fd(80)
 t4.pendown()
 t4.begin_fill()
 t4.fd(50)
 t4.rt(90)
 t4.fd(50)
 t4.rt(90)
 t4.fd(50)
 t4.rt(90)
 t4.fd(50)
 t4.end_fill()
 t4.penup()



 
 




def main(): # The following function is the main function. It is used to call the functions defined previously.
 draw_circle()   
 ground()
 draw_tree(l/2, 2)
 draw_polygon()

main() # This is for calling the main function to execute the functions defined before.

'''THANK YOU FOR REVIEWING THE PROJECT'''
