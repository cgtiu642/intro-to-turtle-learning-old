# Lesson 1: Drawing Lines

## Learning Objectives
- Execute forward and backward motion, and the shorthands of these
- Use basic customization

## Turtle Basics
In Turtle, we can command the cursor to move around to create visual drawings like shapes. The code below instructs the drawing of a line using the command `forward`.

```python
import turtle

s = turtle.getscreen()
t = turtle.Turtle()
t.forward(10)

t.done()
```

The code above moves the cursor forward 10 pixels. Similarly, the command `backward` can move the cursor back 10 pixels.

```python
t.backward(10)
```

Both functions also have shorthand versions `t.fd()` and `t.bk()`, which work in the same way.

The initial angle of the cursor is set to `0` by default. We can change this by using the function `t.setheading()`. For example, the angle can be set to 45 degrees, as shown below.

```python
t.setheading(45)
```

The next functions we will learn about are `t.penup()` and `t.pendown()`. As the function names show, `t.penup()` means the pen is up, so the cursor will not draw anything. When then `t.pendown()` function is used, the cursor will resume drawing.

```python
t.forward(10)
t.penup()
t.backward(10) # this line will not be drawn
t.pendown()
t.forward(10)
```

## Customization
Here are some functions we can use to customize the Turtle screen.

Background color: `t.bgcolor("red")` will change the screen's background color to red. We can also try using "green" or "blue".

Screen title: `t.title("Intro to Turtle")` will change the screen title to "Intro to Turtle", as seen in the top of the window.

Cursor icon: We can change the cursor icon too, using the function `t.shape("turtle")`. There are other options as well, including "arrow", "circle", "square", "triangle", and "classic" (default arrowhead). To hide the cursor, use `t.hideturtle()`.

Cursor size: Finally, we can customize the cursor itself using `t.shapesize()`. `t.shapesize()` takes in 3 parameters: stretch width, stretch length, and outline (e.g. `t.shapesize(1, 5, 10)`).

## Review
Note: Assume we have imported the Turtle module as `t`.

### Question 1
Which command is equivalent to t.backward(90)?  
a. `t.fd(90)`  
b. `t.bk(90)`  
c. `t.rt(90)`  
d. `t.lt(90)`

<details>
<summary>Answer</summary>
b
</details>

### Question 2
What is the purpose of the `t.penup()` command?  
a. Lift the pen, so the turtle doesn't draw  
b. Lower the pen to start drawing  
c. Change the pen color to red  
d. Increase the thickness of the pen

<details>
<summary>Answer</summary>
a
</details>

### Question 3
How do you change the background color of the graphics window to green?  
a. `t.bgcolor("red")`  
b. `t.backgroundcolor("green")`  
c. `t.background("green")`  
d. `t.bgcolor("green")`

<details>
<summary>Answer</summary>
d
</details>

### Question 4
Which command is used to end execution?  
a. `t.done()`  
b. `t.leave()`  
c. `t.exit()`  
d. `t.finish()`

<details>
<summary>Answer</summary>
a
</details>

### Question 5
Which command is used to hide the cursor?  
a. `t.hide()`  
b. `turtle.hide()`  
c. `t.hideturtle()`  
d. `turtle.hideturtle()`

<details>
<summary>Answer</summary>
c
</details>
