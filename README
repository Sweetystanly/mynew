import turtle

def draw_hexagon(side_length):
    for _ in range(6):
        turtle.forward(side_length)
        turtle.left(60)

def draw_honeycomb(columns, rows, side_length):
    turtle.speed("normal")  
    for row in range(rows):
        for col in range(columns):
            draw_hexagon(side_length)
            turtle.penup()
            turtle.forward(side_length * 2)  
            turtle.pendown()
        turtle.penup()
        if row % 2 == 0:
            turtle.goto(0, turtle.ycor() - side_length * 1.75)
        else:
            turtle.goto(-side_length * 1.25, turtle.ycor() - side_length * 1.75)  # Adjust the multiplier for spacing
        turtle.pendown()

rows = int(input("Enter the number of rows: "))
columns = int(input("Enter the number of columns: "))

draw_honeycomb(columns, rows, 50)  # Adjust the side_length as needed
turtle.done()

