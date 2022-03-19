# Old Projects
Here are a couple of projects that I coded earlier in the semester

### Volume Calculator
```
import math
## this program computes the volume of either a cone, cube, or cylinder

def coneVolume():
    height = float(input("Cone Height in Meters: "))
    radius = float(input("Cone Radius in Meters: "))
    volume = round((pow(radius, 2)*(height/3)*math.pi),4)
    print("A cone with height", height, "and radius", radius, "has a volume of", volume, "cubic meters.")

def cubeVolume():
    height = float(input("Cube Height in Meters: "))
    length = float(input("Cube Length in Meters: "))
    width = float(input("Cube Width in Meters:"))
    volume = round((height*width*length),2)
    print("A cube with height", height, "lenght", length, "and width", width, "has a volume of", volume, "cubic meters.")

def cylinderVolume():
    height = float(input("Cylinder Height in Meters: "))
    radius = float(input("Cylinder Radius in Meters: "))
    volume = round((pow(radius, 2)*(height)*math.pi),2)
    print("A cylinder with height", height, "and radius", radius, "has a volume of", volume, "cubic meters.")

def volumeCalculator():
    print("Shape Volume Calculator\n________________________\n1. Calculate the Volume of a Cube\n2. Calculate the Volume of a Cylinder\n3. Calculate the Volume of a Cone")
    calc = int(input("Would you like to perform calculation 1, 2, or 3?: "))

    if (calc == 1):
        cubeVolume()
    if (calc == 2):
        cylinderVolume()
    if (calc == 3):
        coneVolume()
def main():
    print(volumeCalculator())

main()
    
```        
### Turtle Image
```
from turtle import Turtle

sheldon = Turtle()
#this program draws a star using a turtle
sheldon.begin_fill()
sheldon.color("blue")
sheldon.pensize(10)
sheldon.up()
sheldon.setx(0)
sheldon.sety(300)
sheldon.down()
sheldon.seth(180)
sheldon.circle(300)
sheldon.end_fill()
sheldon.seth(288)
sheldon.color("red", "white")
sheldon.begin_fill()
for x in range(5):
    sheldon.fd(571)
    sheldon.right(144)
sheldon.end_fill()
```
----------------------------------------------------------
[Back to Home](README.md "Home")