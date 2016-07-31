# ACD_JAVAB_Session_5_Assignment_1_Main

package OOPsPart3;
public class Sides {
	//parent Class Attributes
	public int side1=10;
	public int side2=20;
}

package OOPsPart3;
public class Triangle extends Sides {
	//child Class "Triangle" method
	public double triArea(){
		return(3.14*side1*side1);
		}
	}


package OOPsPart3;
public class Rectangle extends Sides {
	//child Class "Rectangle" method
	public double recArea(){
		return(side1*side2);
	}
}

package OOPsPart3;
public class SingleInheritance extends Sides {
	public static void main(String[] args) {
		Rectangle r = new Rectangle();    // Create object of child class Rectangle
		Triangle t = new Triangle();     // Create object of child class Triangle
		double aor=r.recArea();         //call method of child class Rectangle
		double aot=t.triArea();        //call method of child class Triangle
		System.out.println("Area of Rectangle is "+aor); //print area of rectangle
		System.out.println("Area of Triangle is "+aot);  //print area of triangle
	}
}
