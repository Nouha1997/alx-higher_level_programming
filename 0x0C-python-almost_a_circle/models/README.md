Models Directory
Models Categories
Base model
Rectangle Model
Square Model
Let's draw it
Let's draw it
Update the class Base by adding the static method def draw(list_rectangles, list_squares): that opens a window and draws all the Rectangles and Squares:

You must use the Turtle graphics module
To install it: sudo apt-get install python3-tk
No constraints for color, shape etc… be creative!
guillaume@ubuntu:~/$ cat 101-main.py
#!/usr/bin/python3
""" 101-main """
from models.base import Base
from models.rectangle import Rectangle
from models.square import Square

if __name__ == "__main__":

    list_rectangles = [Rectangle(100, 40), Rectangle(90, 110, 30, 10), Rectangle(20, 25, 110, 80)]
    list_squares = [Square(35), Square(15, 70, 50), Square(80, 30, 70)]

    Base.draw(list_rectangles, list_squares)

guillaume@ubuntu:~/$ ./101-main.py
....
