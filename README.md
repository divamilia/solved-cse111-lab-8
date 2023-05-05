Download Link: https://assignmentchef.com/product/solved-cse111-lab-8
<br>
<strong> </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="34"><strong>1.</strong></td>

   <td width="532"><strong>class A{ </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>2.</strong></td>

   <td width="532"><strong>  public int temp = 4; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>3.</strong></td>

   <td width="532"><strong>  public int sum = 1; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>4.</strong></td>

   <td width="532"><strong>  public int y = 2; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>5.</strong></td>

   <td width="532"><strong>  public A(){ </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>6.</strong></td>

   <td width="532"><strong>    y = temp – 2; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>7.</strong></td>

   <td width="532"><strong>    sum = temp + 3; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>8.</strong></td>

   <td width="532"><strong>    temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>9.</strong></td>

   <td width="532"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>10.</strong></td>

   <td width="532"><strong>  public void methodA(int m, int n){ </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>11.</strong></td>

   <td width="532"><strong>    int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>12.</strong></td>

   <td width="532"><strong>    y = y + m + (temp++); </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>13.</strong></td>

   <td width="532"><strong>    x = x + 2 +  n; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>14.</strong></td>

   <td width="532"><strong>    sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>15.</strong></td>

   <td width="532"><strong>    System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>16.</strong></td>

   <td width="532"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>17.</strong></td>

   <td width="532"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>18.</strong></td>

   <td width="532"><strong>class B extends A { </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>19.</strong></td>

   <td width="532"><strong>  public int x = 1; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>20.</strong></td>

   <td width="532"><strong>  public int sum = 2; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>21.</strong></td>

   <td width="532"><strong>  public B(){ </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>22.</strong></td>

   <td width="532"><strong>    y = temp + 3 ; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>23.</strong></td>

   <td width="532"><strong>    sum = 3 + temp + 2; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>24.</strong></td>

   <td width="532"><strong>    temp-=1; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>25.</strong></td>

   <td width="532"><strong>  }   </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>26.</strong></td>

   <td width="532"><strong>  public B(B b){ </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>27.</strong></td>

   <td width="532"><strong>    sum = b.sum; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>28.</strong></td>

   <td width="532"><strong>    x = b.x; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>29.</strong></td>

   <td width="532"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>30.</strong></td>

   <td width="532"><strong>  public void methodB(int m, int n){     </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>31.</strong></td>

   <td width="532"><strong>    int  y =0; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>32.</strong></td>

   <td width="532"><strong>    y = y + this.y;  </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>33.</strong></td>

   <td width="532"><strong>    x = this.y + 2 + temp; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>34.</strong></td>

   <td width="532"><strong>    methodA(x, y); </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>35.</strong></td>

   <td width="532"><strong>    sum = x + y + super.sum; </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>36.</strong></td>

   <td width="532"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>37.</strong></td>

   <td width="532"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="34"><strong>38.</strong></td>

   <td width="532"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>    Consider the following code: [Answer on the Question Paper] </strong>

<table width="0">

 <tbody>

  <tr>

   <td rowspan="4" width="295"><strong>A        </strong><strong>a1 = new A(); </strong><strong>B        </strong><strong>b1 = new B(); B b2 = new B(b1); a1.methodA(1, 1); b1.methodA(1, 2); b2.methodB(3, 2); </strong></td>

   <td width="96"><strong>x </strong></td>

   <td width="84"><strong>Y </strong></td>

   <td width="96"><strong>Sum </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

Given the following classes, write the code for the <strong>BBAStudent </strong>class so that the following output is printed when we run the <strong>TestStudent </strong>class.

<strong> </strong>

<strong>Name : Default BBA Student Department: BBA </strong>

<strong>Name : Humty Dumty Department: BBA </strong>

<strong>Name : Little Bo Peep Department: BBA                            </strong>

<strong> </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="639"><strong>public class Student{ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  private String name = “Just a Student”;   </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  private String department = “nothing”; </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  public void setDepartment(String dpt){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    this.department = dpt; </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  protected String getName(){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    return name; </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  protected void setName(String name){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    this.name = name; </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  public String toString(){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    return “Name : ” + name + ” Department: ” + department; </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>public class TestStudent{ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  public static void printName(Student s){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    System.out.println(s.toString()); </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  public static void main(String [] args){ </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    printName(new BBAStudent()); </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    printName(new BBAStudent(“Humty Dumty”)); </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>    printName(new BBAStudent(“Little Bo Peep”));     </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="639"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<h1> [??????????????????????????????????????????]</h1>

Write a java program, which calculates “the area of a circle” and “the volume of a sphere” by overriding the space() method in the subclass. [Extend the following super class ‘Point’ with necessary overriding of specific method. DO NOT CHANGE THE POINT CLASS].                  class Point {                     private double radius;                             Point ( double r) {

radius = r;

}

double space ( ) {

System.out.println(“Space for a Point can’t be defined”);

return 0;

}

protected double getRadius(){

return radius;

}

}

// create new sub class




Implement the above program to include constructors for all the subclasses &amp; use ‘super( )’ to call super-class constructors, if necessary.




<strong><u>Sample </u></strong><strong><u>Input</u></strong><strong><u>/</u></strong><strong><u>Output</u></strong> Enter radius of Circle: <strong>5</strong> Creating a Circle … done!

The area of the Circle is 78.539816339744830961566084581988




Enter radius of Sphere: <strong>7</strong> Creating a Sphere … done!

The area of the Sphere is 205.25072003453315824622603437426













<strong> </strong>




<strong>Design a “Vehicle” class. A vehicle assumes that the whole world is a 2 dimensional graph paper. It maintains its x and y coordinates (both are integers). The vehicle gets manufactured (constructed?) at (0,0) coordinate. </strong>

<strong> </strong>

<strong>Write a user class called “Vehicle”. It must have methods to move up, down, left, right and a toString method for printing current coordinate.  </strong>

<strong> </strong>

<strong>Note: All moves are 1 step. That means a single call to any move method changes value of either x or y or both by 1. </strong>

<strong> </strong>

<strong>Take help from:  http://www.javabeginner.com/learn-java/java-tostring-method http://cscie160-distance.com/toString.html </strong>

<strong> </strong>

public class VehicleUser{     public static void main(String[] args){

Vehicle car = new Vehicle();         System.out.println(car.toString());         car.moveUp();

System.out.println(car.toString());         car.moveLeft();

System.out.println(car.toString());         car.moveDown();

System.out.println(car.toString());         car.moveRight();




<table width="0">

 <tbody>

  <tr>

   <td width="639"> // see, output for following two lines are same because toString() is automatically called. So, you can omit toString when printing.         System.out.println(car.toString());System.out.println(car);}}</td>

  </tr>

  <tr>

   <td width="639"><strong>Expected Output:  </strong>(0, 0)(0, 1)(-1, 1)(-1, 0)(0, 0)(0, 0)</td>

  </tr>

 </tbody>

</table>







<h2>Task 5</h2>

<strong> </strong>

<strong>Design a Vehicle2010 class which inherits movement methods from Task1 and adds new methods called move UpperRight, UpperLeft, LowerRight, LowerLeft. Each of these diagonal move methods must re use two inherited and appropriate move methods. Write user class as well which will show that all of your methods are working. A small user class is shown below as an example. </strong>

<strong> </strong>

<strong>Note: All moves are 1 step. That means a single call to any move method changes value of either x or y or both by 1.  </strong>

<strong> </strong>

Additionally, you have to write an “<strong>equals”</strong> method which tests if significant class properties are same (in this case x and y).

<strong>Take help on “equals” method from: </strong>

<ul>

 <li>http://www.ibiblio.org/java/course/week4/37.html</li>

 <li>http://www.javaworld.com/javaworld/jw-06-2004/jw-0614-equals.html</li>

 <li>http://www.artima.com/lejava/articles/equality.html</li>

</ul>

<strong> </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="639">public class Vehicle2010User{     public static void main(String[] args){Vehicle2010 car = new Vehicle2010();         System.out.println(car);         car.moveLowerLeft();System.out.println(car); Vehicle2010 car2 = new Vehicle2010();         car2.moveLeft();System.out.println(car.equals(car2));         car2.moveDown();System.out.println(car.equals(car2));}}</td>

  </tr>

  <tr>

   <td width="639"><strong>Expected Output: </strong>(0, 0) (-1, -1) false true</td>

  </tr>

 </tbody>

</table>

<strong><em> </em></strong>

<strong><em> </em></strong>

<strong><em> </em></strong>

<strong><em> </em></strong>

<h1>Task 6</h1>

Write the <strong>ComplexNumber</strong> class so that the following code generates the output below:

<table width="0">

 <tbody>

  <tr>

   <td width="551"><strong>public class Tester { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public static void main(String[] args) { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        RealNumber rn = new ComplexNumber(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        System.out.println(rn); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>         </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        System.out.println(“——————–“); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>         </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        rn = new ComplexNumber(5, 7); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        System.out.println(rn); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>         </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        System.out.println(“——————–“); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        ComplexNumber cn = new ComplexNumber(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        cn.check(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>public class RealNumber { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    private double realValue; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public double getRealValue() { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        return realValue; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public void setRealValue(double r) { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        realValue = r; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public RealNumber() { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        this(0); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public RealNumber(double r) { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        setRealValue(r); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public String toString() { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        return “RealPart: “+getRealValue(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public void ping() { </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        System.out.println(“I’m in RealNumber class”); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong>             </strong>

<strong>RealPart: 1.0 </strong>

<strong>ImaginaryPart: 1.0 </strong>

<strong>——————– </strong>

<strong>RealPart: 5.0 </strong>

<strong>ImaginaryPart: 7.0 </strong>

<strong>——————– </strong>

<strong>I’m in ComplexNumber class </strong>

<strong>I’m in RealNumber class </strong>

<strong>Checking ended.</strong>

<strong> </strong>

<h2>Task 7</h2>

Write the <strong>Mango </strong>and the<strong> Jackfruit </strong>classes so that the following code generates the output below:




<table width="0">

 <tbody>

  <tr>

   <td width="551"><strong>public class Test{   </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public static void testFruit(Fruit f){ </strong></td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="551"><strong>        System.out.println(“—-Printing Detail—–“); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        if(f.hasFormalin()){       </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>            System.out.println(“Do not eat the “+f.getName()+”.”); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>            System.out.println(f); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        }else{ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>            System.out.println(“Eat the “+f.getName()+”.”); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>            System.out.println(f); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    }   </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public static void main(String [] args){ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        Mango m = new Mango(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        testFruit(m); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        Jackfruit j = new Jackfruit(); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        testFruit(j); </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>public class Fruit{ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    private boolean formalin = false; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public String name = “”; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public Fruit(boolean formalin, String name){ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        this.formalin = formalin; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        this.name = name;     </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    }     </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public String getName(){ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        return name; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    public boolean hasFormalin(){ </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>        return formalin; </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="551"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>—-Printing Detail—– Do not eat the Mango. </strong>

<strong>Mangos are bad for you </strong>

<strong>—-Printing Detail—– Eat the Jackfruit. </strong>

<strong>Jackfruits are good for you</strong>

<h1>Task 8</h1>

Write the <u>CheckingAccount</u> class so that the following code generates the output below

<strong> </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="591"><strong>public class Account{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  protected double balance = 0.0; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public Account(double balance){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    this.balance = balance; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public double getBalance(){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    return balance; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>public class TestAccount{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public static void printBalance(Account a){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(“Account Balance: ” + a.getBalance()); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public static void main(String [] args) </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  { </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(“Number of Checking Accounts: ” + </strong><strong>CheckingAccount.numberOfAccount); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printBalance(new CheckingAccount()); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printBalance(new CheckingAccount(100.00)); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printBalance(new CheckingAccount(200.00)); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(“Number of Checking Accounts: ” + </strong><strong>CheckingAccount.numberOfAccount); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

<strong>Number of Checking Accounts: 0 </strong>

<strong>Account Balance: 0.0 </strong>

<strong>Account Balance: 100.0 </strong>

<strong>Account Balance: 200.0 </strong>

<strong>Number of Checking Accounts: 3 </strong>

<strong> </strong>

<h1>Task 9</h1>




Write the <strong><u>CSEStudent</u></strong> and <strong><u>CSE111Student</u></strong> class so that the following code generates the output below <strong>[</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="591"><strong>public class Student{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public String msg = “I love BU”; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public String shout(){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    return msg; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>public class TestStudent{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public static void printShout(Student s){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(“——————“); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(s.msg); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(s.shout()); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public static void main(String [] args){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    Student s = new Student(); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    CSEStudent cs = new CSEStudent(); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    CSE111Student cs111 = new CSE111Student(); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(s.msg); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(cs.msg); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(cs111.msg); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printShout(s); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printShout(cs); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    printShout(cs111); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="591"><strong>Output </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>I love BU</strong><strong>I want to transfer to CSE </strong><strong>I love Java Programming </strong><strong>—————— </strong><strong>I love BU </strong><strong>I love BU </strong></td>

  </tr>

 </tbody>

</table>

<strong>—————— </strong>

<strong>I love BU </strong>

<strong>I want to transfer to CSE </strong>

<strong>—————— </strong>

<strong>I love BU </strong>

<strong>I love Java Programming </strong>

<strong> </strong>

<strong> </strong>

<h2>Task 10</h2>

Write the Car class so that the following code generates the output bellow

<strong> public class TestCars{   public static void printCarDetail(Car c){ </strong>

<strong>    System.out.println(“Year: “+ c.getYear()); </strong>

<strong>    System.out.println(“Total Number of Cars: “+ c.getObjectCount()); </strong>

<strong>  }   public static void main(String [] args){ </strong>

<strong>    System.out.println(“Total Number of Cars: “+ </strong>

<strong>Car.getObjectCount()); </strong>

<strong>    System.out.println(“==============================”);     Car c1 = new Car(2000);     printCarDetail(c1);     Car c2 = new Car(2006);     printCarDetail(c2);     Car c3 = new Car(2002);     printCarDetail(c3); </strong>

<strong>    System.out.println(“==============================”);     System.out.println(“Total Number of Cars: “+ </strong>

<strong>Car.getObjectCount());         </strong>

<strong>  } </strong>

<strong>} </strong>




<strong>Total Number of Cars: 0 </strong>

<strong>============================== </strong>

<strong>Year: 2000 </strong>

<strong>Total Number of Cars: 1 Year: 2006 </strong>

<strong>Total Number of Cars: 2 Year: 2002 </strong>

<strong>Total Number of Cars: 3 </strong>

<strong>============================== </strong>

<strong>Total Number of Cars: 3 </strong>




<h2>Task 11</h2>




Given the following classes, write the code for the <strong>Dog </strong>and the<strong> Cat </strong>class so that the following output is printed when we run the <strong>AnimalDriver</strong> class.

<strong>Animal do not make sound meow bark </strong>

<strong> </strong><strong>public class Animal {</strong>

<strong> </strong>

<strong>  //Name of the Animal </strong>

<strong>  private String sound = “Animal Sound”; </strong>

<strong> </strong>

<strong>  //Default Constructor   public Animal(){ </strong>

<strong>  } </strong>

<strong> </strong>

<strong>  //Overloaded Constructor   Animal(String _sound){     this.sound = _sound; </strong>

<strong>  } </strong>

<strong> </strong>

<strong>  //Return sound   public String makeSound(){     return sound; </strong>

<strong>  } </strong>

<strong>}  public class AnimaDriver{ </strong>

<strong>   public static void printSound(Animal a){ </strong>

<strong>    System.out.println(a.makeSound()); </strong>

<strong>  }    public static void main(String [] args){ </strong>

<strong>    Dog d1 = new Dog(“bark”); </strong>

<strong>    Cat c1 = new Cat(“meow”); </strong>

<strong>    Animal a1 = new Animal(“Animal do not make sound”);     printSound(a1);     printSound(c1);     printSound(d1); </strong>

<strong>  } </strong>

<strong>} </strong>

<h2>Task 12</h2>

<table width="0">

 <tbody>

  <tr>

   <td width="495"><strong>class A{ </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public static int temp = 4; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public int sum; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public int y; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public A(){ </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    y = temp – 2; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    sum = temp + 1; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public void methodA(int m, int n){ </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    y = y + m + (temp++); </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    x = x + 1 +  n; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>class B extends A { </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public static int x; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public int sum; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public B(){ </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    y = temp + 3 ; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    sum = 3 + temp + 2; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  }   </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public B(B b){ </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    sum = b.sum; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    x = b.x; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    b.methodB(2,3); </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  public void methodB(int m, int n){     </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    int  y = 0; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    y = y + this.y;  </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    x = this.y + 2 + temp; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    methodA(x, y); </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    sum = x + y + sum; </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="495"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong>Consider the following code: </strong>

<table width="0">

 <tbody>

  <tr>

   <td rowspan="6" width="173"><strong>A        </strong><strong>a1 = new A(); </strong><strong>B        </strong><strong>b1 = new B(); B b2 = new B(b1); b1.methodA(1, 2); b2.methodB(3, 2); </strong></td>

   <td width="96"><strong>x </strong></td>

   <td width="84"><strong>y </strong></td>

   <td width="96"><strong>sum </strong></td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

 </tbody>

</table>




<h2>Task 13</h2>

<table width="0">

 <tbody>

  <tr>

   <td width="591"><strong>class A{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int temp = 4; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int y; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public A(){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = temp – 2; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = temp + 3; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public void methodA(int m, int n){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = y + m + (temp++); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    x = x + 2 +  n; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>class B extends A { </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int x; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public B(){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = temp + 3 ; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = 3 + temp + 2; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    temp-=1; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  }   </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public B(B b){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = b.sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    x = b.x; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public void methodB(int m, int n){     </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    int  y =0; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = y + this.y;  </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    x = this.y + 2 + temp; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    methodA(x, y); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = x + y + sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>Consider the following code: </strong>

<table width="0">

 <tbody>

  <tr>

   <td rowspan="4" width="295"><strong>A        </strong><strong>a1 = new A(); </strong><strong>B        </strong><strong>b1 = new B(); B b2 = new B(b1); a1.methodA(1, 1); b1.methodA(1, 2); b2.methodB(3, 2); </strong></td>

   <td width="96"><strong>x </strong></td>

   <td width="84"><strong>y </strong></td>

   <td width="96"><strong>sum </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

 </tbody>

</table>

<h2>Task 14</h2>

<table width="0">

 <tbody>

  <tr>

   <td width="37">1</td>

   <td width="535"><strong>class A{ </strong></td>

  </tr>

  <tr>

   <td width="37">2</td>

   <td width="535"><strong>  public int temp = 4; </strong></td>

  </tr>

  <tr>

   <td width="37">3</td>

   <td width="535"><strong>  public int sum = 1; </strong></td>

  </tr>

  <tr>

   <td width="37">4</td>

   <td width="535"><strong>  public int y = 2; </strong></td>

  </tr>

  <tr>

   <td width="37">5</td>

   <td width="535"><strong>  public A(){ </strong></td>

  </tr>

  <tr>

   <td width="37">6</td>

   <td width="535"><strong>    y = temp – 2; </strong></td>

  </tr>

  <tr>

   <td width="37">7</td>

   <td width="535"><strong>    sum = temp + 3; </strong></td>

  </tr>

  <tr>

   <td width="37">8</td>

   <td width="535"><strong>    temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="37">9</td>

   <td width="535"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="37">10</td>

   <td width="535"><strong>  public void methodA(int m, int n){ </strong></td>

  </tr>

  <tr>

   <td width="37">11</td>

   <td width="535"><strong>    int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="37">12</td>

   <td width="535"><strong>    y = y + m + (temp++); </strong></td>

  </tr>

  <tr>

   <td width="37">13</td>

   <td width="535"><strong>    x = x + 2 +  n; </strong></td>

  </tr>

  <tr>

   <td width="37">14</td>

   <td width="535"><strong>    sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="37">15</td>

   <td width="535"><strong>    System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="37">16</td>

   <td width="535"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="37">17</td>

   <td width="535"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="37">18</td>

   <td width="535"><strong>class B extends A { </strong></td>

  </tr>

  <tr>

   <td width="37">19</td>

   <td width="535"><strong>  public int x = 1; </strong></td>

  </tr>

  <tr>

   <td width="37">20</td>

   <td width="535"><strong>  public int sum = 2; </strong></td>

  </tr>

  <tr>

   <td width="37">21</td>

   <td width="535"><strong>  public B(){ </strong></td>

  </tr>

  <tr>

   <td width="37">22</td>

   <td width="535"><strong>    y = temp + 3 ; </strong></td>

  </tr>

  <tr>

   <td width="37">23</td>

   <td width="535"><strong>    sum = 3 + temp + 2; </strong></td>

  </tr>

  <tr>

   <td width="37">24</td>

   <td width="535"><strong>    temp-=1; </strong></td>

  </tr>

  <tr>

   <td width="37">25</td>

   <td width="535"><strong>  }   </strong></td>

  </tr>

  <tr>

   <td width="37">26</td>

   <td width="535"><strong>  public B(B b){ </strong></td>

  </tr>

  <tr>

   <td width="37">27</td>

   <td width="535"><strong>    sum = b.sum; </strong></td>

  </tr>

  <tr>

   <td width="37">28</td>

   <td width="535"><strong>    x = b.x; </strong></td>

  </tr>

  <tr>

   <td width="37">29</td>

   <td width="535"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="37">30</td>

   <td width="535"><strong>  public void methodB(int m, int n){     </strong></td>

  </tr>

  <tr>

   <td width="37">31</td>

   <td width="535"><strong>    int  y =0; </strong></td>

  </tr>

  <tr>

   <td width="37">32</td>

   <td width="535"><strong>    y = y + this.y;  </strong></td>

  </tr>

  <tr>

   <td width="37">33</td>

   <td width="535"><strong>    x = this.y + 2 + temp; </strong></td>

  </tr>

  <tr>

   <td width="37">34</td>

   <td width="535"><strong>    methodA(x, y); </strong></td>

  </tr>

  <tr>

   <td width="37">35</td>

   <td width="535"><strong>    sum = x + y + super.sum; </strong></td>

  </tr>

  <tr>

   <td width="37">36</td>

   <td width="535"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="37">37</td>

   <td width="535"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="37">38</td>

   <td width="535"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong>Consider the following code: </strong>

<table width="0">

 <tbody>

  <tr>

   <td rowspan="4" width="295"><strong>A        </strong><strong>a1 = new A(); </strong><strong>B        </strong><strong>b1 = new B(); B b2 = new B(b1); a1.methodA(1, 1); b1.methodA(1, 2); b2.methodB(3, 2); </strong></td>

   <td width="96"><strong>x </strong></td>

   <td width="84"><strong>Y </strong></td>

   <td width="96"><strong>sum </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

 </tbody>

</table>

<h2>Task 15</h2>

<table width="0">

 <tbody>

  <tr>

   <td width="454"><strong>class A{ </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public static int temp = 3; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public int sum; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public int y; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public A(){ </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        y = temp – 1; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        sum = temp + 2; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public void methodA(int m, int [] n){ </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        y = y + m + (temp++); </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        x = x + 2 +  (++n[0]); </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        n[0] = sum + 2; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>} </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>class B extends A { </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public static int x = 1; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public int sum = 2; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public B(){ </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        y = temp + 1 ; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        x = 3 + temp + x; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        temp-=2; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    }   </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public B(B b){ </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        sum = b.sum + super.sum; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        x = b.x + x; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    public void methodB(int m, int n){     </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        int [] y = {0}; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        super.y = y[0] + this.y + m;  </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        x = super.y + 2 + temp – n; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        methodA(x, y); </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        sum = x + y[0] + super.sum; </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>        System.out.println(x + ” ” + y[0]+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>    } </strong></td>

  </tr>

  <tr>

   <td width="454"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

<strong>Consider the following code: </strong>

<table width="0">

 <tbody>

  <tr>

   <td rowspan="3" width="295"><strong>int x[] = {23}; A a1 = new A(); </strong><strong>B b1 = new B(); </strong><strong>B b2 = new B(b1); </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="84"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td rowspan="2" width="295"><strong>a1.methodA(1, x); b2.methodB(3, 2); a1.methodA(1, x); </strong></td>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

  <tr>

   <td width="96"> </td>

   <td width="84"> </td>

   <td width="96"> </td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<h2>Task 16</h2>

<table width="0">

 <tbody>

  <tr>

   <td width="591"><strong>public class FinalT6A{ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public static int temp = 4; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  private int sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  private int y = 1; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public FinalT6A(int x, int p){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    temp+=1; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = temp – p; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = temp + x; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public void methodA(){     </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    int x=0, y =0; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = y + this.y;  </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    x = this.y + 2 + temp; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = x + y + methodB(temp, y); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(x + ” ” + y+ ” ” + sum); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  public int methodB(int temp, int n){ </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    int x = 0; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    y = y + (++temp); </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    x = x + 3 +  n; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    sum = sum + x + y; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    System.out.println(x + ” ” + y+ ” ” + sum);   </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>    return sum; </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>  } </strong></td>

  </tr>

  <tr>

   <td width="591"><strong>} </strong></td>

  </tr>

 </tbody>

</table>

What is the output of the following code sequence?




<table width="0">

 <tbody>

  <tr>

   <td rowspan="8" width="307"><strong>FinalT6A q1 = new FinalT6A(2,1); q1.methodA(); q1.methodA();   </strong></td>

   <td width="96"><strong>x </strong></td>

   <td width="96"><strong>y </strong></td>

   <td width="91"><strong>sum </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

  <tr>

   <td width="96"><strong> </strong></td>

   <td width="96"><strong> </strong></td>

   <td width="91"><strong> </strong></td>

  </tr>

 </tbody>

</table>







<h3><strong><u>Task 17</u></strong></h3>

<strong>Mutant Flatworld Explorers </strong>http://online-judge.uva.es/p/v1/118.html

<strong>Hint:</strong> It is similar to Task 1 and 2 but here you will have to maintain a two dimensional character array

<em> </em>

<h3>Background</h3>

Robotics, robot motion planning, and machine learning are areas that cross the boundaries of many of the subdisciplines that comprise Computer Science: artificial intelligence, algorithms and complexity, electrical and mechanical engineering to name a few. In addition, robots as “turtles” (inspired by work by Papert, Abelson, and diSessa) and as “beeper-pickers” (inspired by work by Pattis) have been studied and used by students as an introduction to programming for many years.




This problem involves determining the position of a robot exploring a pre-Columbian flat world.

<em> </em>

<h3>The Problem</h3>

Given the dimensions of a rectangular grid and a sequence of robot positions and instructions, you are to write a program that determines for each sequence of robot positions and instructions the final position of the robot.




A robot <em>position</em> consists of a grid coordinate (a pair of integers: x-coordinate followed by ycoordinate) and an orientation (N,S,E,W for north, south, east, and west). A robot <em>instruction</em> is a string of the letters ‘<em>L</em>‘, ‘<em>R</em>‘, and ‘<em>F</em>‘ which represent, respectively, the instructions:




<ul>

 <li><em>Left</em>: the robot turns left 90 degrees and remains on the current grid point.</li>

 <li><em>Right</em>: the robot turns right 90 degrees and remains on the current grid point.</li>

 <li><em>Forward</em>: the robot moves forward one grid point in the direction of the current orientation and mantains the same orientation.</li>

</ul>




The direction <em>North</em> corresponds to the direction from grid point (<em>x</em>,<em>y</em>) to grid point (<em>x</em>,<em>y</em>+1).  Since the grid is rectangular and bounded, a robot that moves “off” an edge of the grid is lost forever. However, lost robots leave a robot “scent” that prohibits future robots from dropping off the world at the same grid point. The scent is left at the last grid position the robot occupied before disappearing over the edge. An instruction to move “off” the world from a grid point from which a robot has been previously lost is simply ignored by the current robot.

<em> </em>

<em>Hint: For your convenience, you may mark cells having the scent with ‘X’ or any character you like</em><em> to mean forbidden cells. </em>

<em> </em>

<h3>The Input</h3>

The first line of input is the upper-right coordinates of the rectangular world, the lower-left coordinates are assumed to be 0,0.




The remaining input consists of a sequence of robot positions and instructions (two lines per robot). A position consists of two integers specifying the initial coordinates of the robot and an orientation (N,S,E,W), all separated by white space on one line. A robot instruction is a string of the letters ‘L’, ‘R’, and ‘F’ on one line.




Each robot is processed sequentially, i.e., finishes executing the robot instructions before the next robot begins execution.




Input is terminated by end-of-file.




You may assume that all initial robot positions are within the bounds of the specified grid. The maximum value for any coordinate is 50. All instruction strings will be less than 100 characters in length.

<h3>The Output</h3>

For each robot position/instruction in the input, the output should indicate the final grid position and orientation of the robot. If a robot falls off the edge of the grid the word “LOST” should be printed after the position and orientation.

<em> </em>

<em>Sample Input </em>

<h2>5 3 1 1 E RFRFRFRF 3 2 N</h2>

<h2>FRRFLLFFRRFLL 0 3 W LLFFFLFLFL</h2>

<em> </em>

<em>Sample Output </em>

<h2>1 1 E</h2>

3 3 N LOST 2 3 S