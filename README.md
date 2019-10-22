# Area-Reader
The area reader file is a code that is written in the Java language that has the capability to read out the area of certain shapes that are instilled in the code. There are six different files contained in this project; Circle.java, Rectangle.java, Triangle.java, Point.java, Shape.java, and Main.java. The files that are named after shapes are files that contain classes that each contain the algorithm to compute the area of each shape that it is named after. Each of the classes contains variables of each of the constants that are needed to calculate the area for each shape. All of the variables are defined as doubles so the values that are taken into consideration can be values that contain decimal values.

Triangle contains: (1/2(B)(H))

Base

Height

Rectangle contains: (L(W))

Length

Width

Circle contains:(Pi(r^2))

Radius

The triangle class extends the the Shape class which is defined in another file. The triangle class presets the points of the shape to 0 as well as the base and the height. As the main process file is being ran, the predefined values that are assigned to the triangle class are being run through the getBase() and getHeight() methods. The getBase() and getHeight() methods pull the values defined from the main class and bring it to triangle.java. The final process in determining the area of the triangle is to initiate the following code

return(this.base * this.height)/2

The proceeding line changes all of the variables into string form and return each of the variables in their numberical form in this order:

(x,y,z) : /triangle area\
