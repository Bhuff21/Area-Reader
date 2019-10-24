# ReadMe
The area reader file (Lab5c) is a code that is written in the Java language that has the capability to read out the area of certain shapes that are instilled in the code. There are six different files contained in this project; Circle.java, Rectangle.java, Triangle.java, Point.java, Shape.java, and Main.java. The files that are named after shapes are files that contain classes that each contain the algorithm to compute the area of each shape that it is named after. Each of the classes contains variables of each of the constants that are needed to calculate the area for each shape. All of the variables are defined as doubles so the values that are taken into consideration can be values that contain decimal values.

Triangle contains: (1/2(B)(H))

Base

Height

Rectangle contains: (L(W))

Length

Width

Circle contains:(Pi(r^2))

Radius

The triangle class extends the Shape class which is defined in the shape file. The triangle class presets the points of the shape to 0 as well as the base and the height. As the main process file is being ran, the predefined values that are assigned to the triangle class are being run through the getBase() and getHeight() methods. The getBase() and getHeight() methods pull the values defined from the main class and bring it to triangle.java file. The final process in determining the area of the triangle is to initiate the following code

return(this.base * this.height)/2

The proceeding line changes all of the variables into string form and return each of the variables in their numberical form in this order:

public String toString(){
  return "(" + getX() + ", " + getY() + ", " + getZ() + ")" + ":" + "(" + this.area() + ")";
}

(x,y,z) : /triangle area\

The rectangle class extends the Shape class which is also defined in the shape file. The rectangle class presets the points of the shape to 0 as well as the length and width. As the main process file is being ran, the predefined values that are assigned to the rectangle class are being run through the getLength() and getWidth() methods. The getLength() and getwidth() methods pull the values defined from the main class and bring it to rectangle.java file. The final process in determining the area of the rectangle is to initiate the following code

return this.length * this.width

The proceeding line changes all of the variables into string form and return each of the variables in their numberical form in this order:

 public String toString(){
        return "(" + getX() + ", " + getY() + ", " + getZ() + ")" + ":" + "[" + this.area() + "]";

(x,y,z) : [rectangle area]

The circle class extends the Shape class which is also defined in the shape file. The circle class presets the points of the shape to 0 as well as the radius. As the main process file is being ran, the predefined values that are assigned to the circle class are being run through the getRadius method. The getRadius() method pulls the values defined from the main class and bring it to circle.java file. The final process in determining the area of the circle is to initiate the following code:

return Math.PI * (this.radius * this.radius);

The proceeding line changes all of the variables into string form and return each of the variables in their numberical form in this order:

 public String toString(){
        return "(" + getX() + ", " + getY() + ", " + getZ() + ")" + ":" + "(" + this.area() + ")";
    }

(x,y,z) : (Circle area)

The shape file is a super class to the rest of the shapes, it gathers all of the points from the main file from each shape and extracts them to their rightful shape file. It also helps find the center of each shape with he points that are provided in the main file. The first three numbers that are defined in the main after the shapes name are the points that each shape is accepting. Here is an example of what it will look like.

Rectangle rectangle = new Rectangle(5,5,5, 4.0, 10.0);

The point file sets the points for the variables X, Y, and Z so that they are within the bounds defined by the shapes so if the value of any point is less than 0, it is set to a default value of 0 and if the value of a point is greater than 500 then the variable is set to a default value of 500. Then after each point is set to its value it is sent to its correct file and stored in the variables with labels of each point.

The main file basically lays out all the values that need to be calculated and in what format that the output needs to be laid out in. It brings in all the solutions to the areas of each shape as a string.

The second file is a file that has the capabilities of finding the smallest, largest, and average number that is input from the user through the keyboard. There are four different variables that are kept up throughout the entire code and they are:

int smallestNumber which taking into the account of what the user is inputing and checking to see if it is less than the number that is already in the value of the variable. At the beginning of the code, the smallest value is set to 101 since the values that are needing to be used are between 1 and 100.

int largestNumber which taking into the account of what the user is inputing and checking to see if it is more than the number that is already in the value of the variable. At the beginning of the code, the largest value is set to 0 since the values that are needing to be used are between 1 and 100.

int totalValue takes a running total of all the values entered in by the user and at the end of the code is divided by the amount of inputs that were taken in from the keyboard to calculate the average that is held in the variable double averageNumber.

Int currentNumber is the number that is the last recorded value from the keyboard from the user.

The value are each taken in one by one through the for loop that is under the scanner and is separated into its correct variable and if it is not needed in one of the variable then it is thrown out. After the process has occurred, each of the value are present is an ordered fashion the follows the in this order: Smallest number, Largest Number, and the average.
