# Javastuff

/*
 * Karen Toubbeh
 * CS A170
 * February 1,2017
 * 
public class __SHELL0 extends bluej.runtime.Shell {
public static void run() throws Throwable {

java.lang.String[] __bluej_param0 = { };
Stars.main(__bluej_param0);

}}

/*
 * Karen Toubbeh
 * CS A170
 * February 27, 2017
 *
 * Exercise #10
 */


import java.util.Scanner;
class Digits
{
   public static void main(String args[])
   {
      int num=0;
      int reverseNum =0;
      int i = 0;
      
      
      
      System.out.println("Input your number and press enter: ");
      //This statement will capture the user input
      Scanner in = new Scanner(System.in);
      //Captured input would be stored in number num
      num = in.nextInt();
      //While Loop: Logic to find out the reverse number
      while( num != 0 )
      {
          reverseNum = reverseNum * 10;
          reverseNum = reverseNum + num%10;
          num = num/10;
      }

      System.out.println("Reverse of input number is: "+reverseNum);
      
    
      
   { 
       
      
      System.out.println("\nSum of numbers is = " + reverseNum + i);
   }
   
      
  
}
   
}

/*
 * Karen Toubbeh
 * CS A170
 * February 27, 2017
 *
 * Exercise #10
 */


import java.util.Scanner;
 
public class ForLoops
{
public static void main(String[] args) {
    
    

    Scanner input = new Scanner(System.in);

int count = 0;
 


    
    
    System.out.println("Enter an integer: ");
    int start = input.nextInt();
    
    System.out.println("Enter another integer larger than the first one: ");
    int end = input.nextInt();
    
    
    
    int evenSum = 0;
    System.out.print("Even numbers: ");
    for (int i = start; i <= end; ++i)
    {

        
    if (i % 2 == 0)
    {
        
        System.out.print(+i + " ");
        evenSum +=i;
    }
    
    
     }
 

  
    
     System.out.println("\nSum of even numbers is: " + evenSum);
    
    
    
    
    
    
    
    
    int oddSum = 0;
    System.out.print("Odd numbers: ");
    for (int i = start; i <= end; ++i)
    {

        
    if (i % 2 == 1)
    {
        
        System.out.print(+i + " ");
        oddSum +=i;
    }
    
    
     }
 

  
    
     System.out.println("\nSum of odd numbers is: " + oddSum);




    }
}




/*
 * Karen Toubbeh
 * CS A170
 * February 27, 2017
 *
 * Exercise #10
 */


import java.util.Scanner;
 
public class Stars
{
public static void main(String[] args) {
    
    

    Scanner input = new Scanner(System.in);

int count = 0;
 


    
    
    System.out.println("Enter an integer from 3 to 10: ");
    int start = input.nextInt();
    
      
    int end = input.nextInt();
    
    int stars = input.nextInt();
    
  
    System.out.print("*");
    for (int i = start; i <= end; ++i)
    {

        
    if (i % 2 == 0)
    {
        
        System.out.print(+i + " ");
        stars +=i;
    }
    
    
     }
 

  
    
     System.out.println("+stars");
    
    
    
    
    
    




    }
}




/*
 * Karen Toubbeh
 * CS A170
 * February 27, 2017
 *
 * Exercise #10
 */


import java.util.Scanner;
 
public class WhileLoops
{
    public static void main(String[] args) 
{
    
    

    Scanner input = new Scanner(System.in);

    int count = 0;
 


        System.out.println("Enter an integer: ");
		int x = input.nextInt();
		
		System.out.println("Enter another integer larger than the first one: ");
		int y = input.nextInt();
		
		
		int sumE=0;
		int sumO=0;
		int i = x;
		
		System.out.print("\nEven numbers: ");
		while (i<=y)
		{
			if (i%2==0)
			{
				sumE = sumE + i;
				System.out.print(i + " ");
			}
			i++;/*
 * Karen Toubbeh 
 */
public class MyArray_ABC
{
    public static void main(String[] args)
    {
        //int[] a = {10,20,30,40,50};
        //int[] a = {45, 38, 27, 46, 81, 72, 56, 61, 20, 48, 76, 91, 57, 35, 78};
        int[] a = {45, 38, 27, 46, 81, 72, 56, 61, 20, 48, 76, 91, 57, 35, 800};
        int maxValue = a[0];
        int maxIndex = 0; 
        int sum = 0; 
        for (int idx =1; idx < a.length; idx++)
        
        {
            if (a[idx] > maxValue)
            {
                maxValue = a[idx];
                maxIndex = idx; 
               
            }
            sum += a[idx];
        }
        System.out.println("The largest element is" +maxValue);
        System.out.println("The largest element is at index" +maxIndex);
        System.out.println("The sum of all elements is:" +sum);
    }
}
/*
 * Karen Toubbeh 
 */
public class MyArray_DE
{
    public static void main(String[] args)/**
 * Karen Toubbeh
 * CS 170 
 * March 20, 2017 
 */

class ArrayRange { 
 
  public static void main(String args[]){
    int array[] = new int[]{7, 15, 9, 4, 12, 100};
 
    
    int max = Max(array);
    System.out.println("Maximum Value is: "+max);
 
   
    int min = Min(array);
    System.out.println("Minimum Value is: "+min);
  }
 
  
  public static int Max(int[] inputArray){ 
    int maxValue = inputArray[0]; 
    for(int i=1;i < inputArray.length;i++){ 
      if(inputArray[i] > maxValue){ 
         maxValue = inputArray[i]; 
      } 
    } 
    return maxValue; 
  }
 
  
  public static int Min(int[] inputArray){ 
    int minValue = inputArray[0]; 
    for(int i=1;i<inputArray.length;i++){ 
      if(inputArray[i] < minValue){ 
        minValue = inputArray[i]; 
      } 
    } 
    return minValue; 
  } 
}
/**
 * Karen Toubbeh
 * CS 170 
 * March 20, 2017 
 */

public class ArraysAndLoops
{
    public static void main(String[] args)
    {
        //1. Declare an array arr1 and initialize it to 1, 2, 3, 4, 5, 6, 7, 8, and 9
        int[] arr1 = {1, 2, 3, 4, 5, 6, 7, 8, 9};
        
        //2. Declare another array arr2, the same length as arr1, without giving it any initial values.
        int[] arr2 = new int[arr1.length];
        
        //3. Using a for loop print arr1 displaying all elements on one line, separated by a comma.
        for (int i =0; i < arr1.length; i++)
        {
            //if (i != arr1.length - 1)
                System.out.print(arr1[i] + ",");
            //else
             //   System.out.print(arr1[i]);
            
        }
        System.out.println("arr1[arr1.length-1]");
        
        
        //4. Using a while loop print arr2 displaying all elements on one line, separated by a dash.
        int idx =0;
        while (idx < arr2.length)
        {
            idx++;
        }
        System.out.println("");
        
        
        //5. Using a for loop, copy all the values of arr1 into arr2 in reverse order. 
        for (int i = arr1.length - 1; i >= 0; --i)
        {
            System.out.println(arr1[i]);
        }
        
        //6. Using a do/while loop, print arr1 displaying all elements on one line, separated by a comma.
        
        
        //7. Using a for loop, print arr2 displaying all elements on one line, separated by a dash.
        
        
    }
}

/**
 * Karen Toubbeh
 * CS 170 
 * March 20, 2017 
 */


import java.util.Scanner;

public class Passwords
{
    public static final String[] usernames = {"ptran", "csmith", "bwhite", "abrown","kt"  };
    public static final String[] userpassword = {"123", "xyz", "678", "345", "456"};
    
  

public static void main(String [] args)
{
    Scanner input = new Scanner(System.in);
    int[] list = new int[20];
    
    System.out.println("Please enter your username.");
   
        
    String userN = input.next();
    
        
    boolean found = false; 
    
    int i = 0;
    
    
        while (! found && i < usernames.length )
        {
            if (userN.equals(usernames))
                found = true;
                
                else i++;
            
        }
        
        i = 0; 
        
        if (! found )
        {
            System.out.println("Please enter your username.");
            
   
        
            String usernames = input.next();
          
            while (! found && i < usernames.length())
            {
                if (userN.equals(usernames))
                    found = true;
            
            }
        }
        
        if ( ! found ) 
        {
            System.out.println("Wrong, contact administrator");
        }
            
      else 
        {
            
        
    
        }
    }
        
        
        
        
        
        
        
        
        
        
        
        
        
        
    System.out.println("Please enter your username.");
    System.out.println("Please enter your password.");
    
    
    userN = input.nextInt();
    
    while (userN > 0 )
    {
          boolean found = false; 
            int idx = 0;
            while (!found && idx < userPass)
            {
                if (list[idx] == userN)
                {
                    found = true;
                }
                else
                {
                    ++idx;
                }
            }
            
            
            if (found)
                System.out.println("You may proceed");
            else
                System.out.println("Wrong username and/or password.");
            
            
            userN = input.nextInt();
    }
        /*
 * Class Testing
 * 
 * Do NOT modify this file.
 * 
 */

public class Testing
{
    
    public static void main (String[] args)
    {
       // ******************* DO NOT MODIFY THE MAIN METHOD******************* 
              
       testA();
       testB();
       testC();
       testD();
       testE();
       testF();
       testG();
    }
    
    public static void testA()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION A\n");
       
       YourCode a = new YourCode();
         
       a.sectionA("WooHoo");
       a.sectionA("HelloThere");  
       a.sectionA("abcdef");   
       a.sectionA("ab");   
       a.sectionA("0123456789");   
       a.sectionA("kitten");
    }
    
    public static void testB()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION B\n");
              
       YourCode b = new YourCode();
              
       b.sectionB("Hello");    
       b.sectionB("java");     
       b.sectionB("coding");   
       b.sectionB("code");    
       b.sectionB("ab");    
       b.sectionB("Chocolate!");
       b.sectionB("kitten");
       b.sectionB("woohoo");
    }
    
    public static void testC()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION C\n");
       
       YourCode c = new YourCode();
      
       c.sectionC("Hello","hi");  
       c.sectionC("hi","Hello"); 
       c.sectionC("aaa","b");    
       c.sectionC("b","aaa");  
       c.sectionC("aaa","1234");  
       c.sectionC("aaa","bb"); 
       c.sectionC("a","bb");    
       c.sectionC("bb","a"); 
       c.sectionC("xyz","ab");
    }
    
    public static void testD()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION D\n");
       
       YourCode d = new YourCode();
     
       d.sectionD("Hello","There"); 
       d.sectionD("java","code"); 
       d.sectionD("shotl","java"); 
       d.sectionD("ab","xy"); 
       d.sectionD("ab","x"); 
       d.sectionD("x","ac"); 
       d.sectionD("a","x"); 
       d.sectionD("kit","kat"); 
       d.sectionD("mart","dart"); 
    }
    
    public static void testE()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION E\n");
       
       YourCode e = new YourCode();
  
       e.sectionE("Hello"); 
       e.sectionE("java");
       e.sectionE("Hi");
       e.sectionE("code");
       e.sectionE("cat");
       e.sectionE("12345");
       e.sectionE("Chocolate");
       e.sectionE("bricks");
    }
    
    public static void testF()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION F\n");
       
       YourCode f = new YourCode();
   
       f.sectionF("string");
       f.sectionF("code");
       f.sectionF("Practice");
       f.sectionF("ab");
       f.sectionF("0123456789");       
    }
    
    public static void testG()
    {
       System.out.println("\n**********************************************************");
       System.out.println("TESTING SECTION G\n");
       
       YourCode g = new YourCode();
   
       g.sectionG("abc hi ho");
       g.sectionG("ABChi hi");
       g.sectionG("hihi");
       g.sectionG("hiHIhi");
       g.sectionG("h");
       g.sectionG("hi");
       g.sectionG("Hi is no HI on ahI");
       g.sectionG("hiho not HOHIhi");
    }
}
    

/*
 * Karen Toubbeh
 * Exercise 19
 * April 5, 2017 
 * CS 170
 */

import java.util.Scanner;

public class YourCode
{
    public static Scanner input = new Scanner(System.in);

    public YourCode(){}
    
    public static void sectionA(String str)
    {
        
        str.substring(0, str.length() / 2);
       
       

    }
    
    public static void sectionB(String str)
    {
        String str = "";
        char first = String.charAt(0);
        char last = String.charAt(String.length() - 1);
        
        
    
    }
    
    public static void sectionC(String str1, String str2)
    {
        String str = "";
        String sentence;
        sentence = str.concat ("");
        System.out.println(sentence);
        
  
    }
    
    public static void sectionD(String str1, String str2)
    {
        String str = "";
        char first = String.charAt(0);
        
   
    }
    
    public static void sectionE(St/**
 * Karen Toubbeh
 * CS A170
 * 
 */

public class Rectangle
{
   // private fields
   private double width;
   private double length;   
   
   // Default constructor
   public Rectangle()
   {
       width = 0.0;
       length = 0.0;       
    }
   
   // Overloaded constructor
   public Rectangle(double newWidth, double newLength)
   {
       width = newWidth;
       length = newLength;
       
    }
   
   // Methods
   public double getWidth ()
   {
       return width; 
    }
    
   public double getLength ()
   {
       return length;        
    }
    
   public void setWidth (double newWidth)
   {
       width = newWidth;
    }
   
   public void setLength(double newLength)
   {
       length = newLength;
    }

   public double getArea()
   {
	  double area = length * width;
	  return area;
	}
	
	 public double getPerimeter ()
   {
	    return (length + width) * 2;
	}
	
	 public void printDimensions()
   {
	    System.out.printf("Width: %.2f\n" ,width);
	    System.out.printf("Length: %.2f\n" ,length);
	    
	    
	}

   
}


/**
 * Karen Toubbeh 
 * CS A170 
 */

public class RectangleTest
{
    public static void main(String[] args)
    {/*
 * DigiPet class - digital pet
 * 
 * Karen Toubbeh
 * CS A170
 * Exercise 26
 * May 1, 2017 
 */

public class DigiPet
{
    // instance variables (representing the attributes/state of a DigiPet)
    private String name;
    private int lifespan;   // max age (in cycles)
    private int age;        // current age (in cycles, each action performed causes a cycle to pass)
    private int mood;       // (2 = joyful, 1 = happy, 0 = neutral, -1 = sad, -2 = angry)
    private int size;

    // Default constructor
    public DigiPet()
    {
        name = "(animal)";
        lifespan = 12;
        age = 0;
        size = 1;
        mood = 0;
    }

    // Overloaded constructor
    public DigiPet(String newName, int newLifespan, int newAge, int newMood, int newSize)
    {
        // Initialize all five fields as appropriate:
        // Your code here:
        name = newName; 
        lifespan = newLifespan;
        age = newAge;
        mood = newMood;
        size = newSize;
        
    }

    // Makes a pet one cylcle older and checks if the pet is at the end of its life
    private void makeOlder()
    {
        age++;
        if (age >= lifespan)
        {
            name = "Zombie " + name;
        }
    }
    
    // Accessor method for age
    public int getAge()
    {
        return age;
    }
    
    // Accessor method for lifespan
    public int getLifespan()
    {
        return lifespan;
    }
    
    public void poke()
    {
        // Your code here
        mood--;
        if (mood < -2 )
        mood = -2; 
        
        makeOlder();
        
    }

    public void pet()
    {
        // Your code here
        mood++;
        if (mood > 2)
        mood = 2;
        
        makeOlder();
        
       
      
        
    }
    
    public void feed(int amount)
    {
        // Your code here
        size+= amount;
        
        makeOlder();
        
    }

    public void exercise(int amount)
    {
        // Your code here
        size-=amount;
        
        if ( size < 1 )
        {
            System.out.print("No more energy!");
            size = 1;
            
        
        }
        makeOlder();
    }

    // Modify this method to customize your pet's "appearance"
    public void showPet()
    {
        System.out.println(name + " (" + age + "/" + lifespan + ")");
        
        System.out.print("(\\_");  // ears
        for (int i = 0; i < size; i++)
        {
            System.out.print("_");
            
        }
        System.out.println("__/)");
        
        
        
       
         // face
         System.out.print("(' ");
        for (int i = 0; i < size; i++)
        {
            
            System.out.print("X ");
        }
        
        System.out.println("' )");
        
        
        // tail and feet 
        System.out.print("C(\")");
        for (int i = 0; i < size; i++)
        {
             System.out.print(" (\")");
        }
        
        
        
        
        System.out.print(" --(i'm so ");
        switch (mood)
        {
            case 2: System.out.print("joyful!"); break;
            case 1: System.out.print("happy"); break;
            case -1: System.out.print("sad"); break;
            case -2: System.out.print("angry!"); break;
            default: System.out.print("meh");
        }
        System.out.println(")");
    }
}

/*
 * DigiPet tester program
 */

import java.util.Scanner;

public class DigiPetTester
{
    static Scanner input = new Scanner(System.in);
    
    public static void main(String[] args)
    {
        System.out.print("Enter DigiPet name: ");
        String petName = input.next();
        System.out.print("Enter lifespan: ");
        int petLifespan = input.nextInt();
        
        DigiPet myPet = new DigiPet(petName, petLifespan, 0, 0, 1);
        
        boolean keepGoing = true;
        while (myPet.getAge() <= myPet.getLifespan() && keepGoing)
        {
            System.out.println();
            myPet.showPet();
            
            System.out.print("\n(P)et, po(K)e, (F)eed, (E)xercise, (Q)uit: ");
            String userCommand = input.next();
            char command = userCommand.charAt(0);
            switch (command)
            {
                case 'P':
                case 'p':
                    myPet.pet();
                    break;
import javax.swing.JApplet;
import java.awt.Graphics;
import java.awt.Color;

/**
 * Class Snowman - write a description of the class here
 * 
 * Karen Toubbeh
 * CS A170 Exercise 28
 * May 15, 2017 
 */
public class Snowman extends JApplet
{
    //SUN
    public static final int SUN_DIAMETER = 75;
    public static final int X_SUN = 25;
    public static final int Y_SUN = 15;
    
    // GRAY RECTANGLE 
    public static final int width = 500; 
    public static final int X_RECT = 0;
    public static final int Y_RECT = 400;
    public static final int height = 100;
    
    //FACE
    public static final int FACE_DIAMETER = 50; 
    public static final int X_FACE = 227;
    public static final int Y_FACE = 210;
    
    //MIDDLE
    public static final int MIDDLE_DIAMETER = 80; 
    public static final int X_MIDDLE = 210;
    public static final int Y_MIDDLE = 250;
    
    //LOW 
    public static final int LOW_DIAMETER = 100; 
    public static final int X_LOW = 200;
    public static final int Y_LOW = 300;
    
    //Left eye
    public static final int Leye_DIAMETER = 10; 
    public static final int X_Leye = 235;
    public static final int Y_Leye = 225;
    
    //Right eye
    public static final int Reye_DIAMETER = 10; 
    public static final int X_Reye = 255;
    public static final int Y_Reye = 225;
    
    //Left arm
    public static final int Lx1 = 165;
    public static final int Ly1 = 245;
    public static final int Lx2 = 220;
    public static final int Ly2 = 285;
    
    //Right arm
    public static final int Rx1 = 285;
    public static final int Ry1 = 285;
    public static final int Rx2 = 330;
    public static final int Ry2 = 315;
    
    //mouth 
    public static final int Mx1 = 245;
    public static final int My1 = 245;
    public static final int Mx2 = 260;
    
   // Hat Base
    public static final int hWidth = 55; 
    public static final int X_hat = 225;
    public static final int Y_hat = 210;
    public static final int hHeight = 7; 
    
    // Top Hat Rectangle
    public static final int tWidth = 45; 
    public static final int X_top = 230;
    public static final int Y_top = 170;
    public static final int tHeight = 40;
    
    
    public void init()
    {
        setBackground(Color.BLUE); 
    }
   
   public void paint (Graphics canvas)
   {
       //Sun 
       canvas.setColor(Color.YELLOW);
       canvas.fillOval(X_SUN, Y_SUN, SUN_DIAMETER, SUN_DIAMETER);
       
       //Gray Rect
       canvas.setColor(Color.DARK_GRAY);
       canvas.fillRect(X_RECT, Y_RECT, width, height );
       
       //Face 
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_FACE, Y_FACE, FACE_DIAMETER, FACE_DIAMETER);
       
       //middle body 
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_MIDDLE, Y_MIDDLE, MIDDLE_DIAMETER, MIDDLE_DIAMETER);
       
       //lower body
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_LOW, Y_LOW, LOW_DIAMETER, LOW_DIAMETER);
       
       //left eye
       canvas.setColor(Color.BLACK);
       canvas.fillOval(X_Leye, Y_Leye, Leye_DIAMETER, Leye_DIAMETER);
       
       //right eye 
       canvas.setColor(Color.BLACK);
       canvas.fillOval(X_Reye, Y_Reye, Reye_DIAMETER, Reye_DIAMETER);
       
       //left arm
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Lx1, Ly1, Lx2, Ly2 ); 
       
       //right arm
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Rx1, Ry1, Rx2, Ry2 ); 
       
       //Mouth
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Mx1, My1, Mx2, My1 ); 
  
       //Hat Base
       canvas.setColor(Color.BLACK);
       canvas.fillRect(X_hat, Y_hat, hWidth, hHeight );
       
       //Top Hat
       canvas.setColor(Color.BLACK);
       canvas.fillRect(X_top, Y_top, tWidth, tHeight );
   }
   
   
}


import javax.swing.JApplet;
import java.awt.Graphics;
import java.awt.Color;

/**
 * Class Snowman - write a description of the class here
 * 
 * Karen Toubbeh
 * CS A170 Exercise 28
 * May 15, 2017 
 */
public class Snowman2 extends JApplet
{
    //SUN
    public static final int SUN_DIAMETER = 75;
    public static final int X_SUN = 375;
    public static final int Y_SUN = 25;
    
    
    
    // GRAY RECTANGLE 
    public static final int width = 500; 
    public static final int X_RECT = 0;
    public static final int Y_RECT = 400;
    public static final int height = 100;
    
    //FACE
    public static final int FACE_DIAMETER = 50; 
    public static final int X_FACE = 250;
    public static final int Y_FACE = 210;
    
    //MIDDLE
    public static final int MIDDLE_DIAMETER = 80; 
    public static final int X_MIDDLE = 230;
    public static final int Y_MIDDLE = 250;
    
    //top button
    public static final int topB_DIAMETER = 10; 
    public static final int X_tButton = 265;
    public static final int Y_tButton = 265;
    
    //bottom button 
    
    public static final int bottomB_DIAMETER = 10; 
    public static final int X_bButton = 265;
    public static final int Y_bButton = 280;
    
    //LOW 
    public static final int LOW_DIAMETER = 100; 
    public static final int X_LOW = 220;
    public static final int Y_LOW = 300;
    
    //Left eye
    public static final int Leye_DIAMETER = 10; 
    public static final int X_Leye = 255;
    public static final int Y_Leye = 225;
    
    //Right eye
    public static final int Reye_DIAMETER = 10; 
    public static final int X_Reye = 275;
    public static final int Y_Reye = 225;
    
    //Left arm
    public static final int Lx1 = 185;
    public static final int Ly1 = 245;
    public static final int Lx2 = 240;
    public static final int Ly2 = 285;
    
    //Right arm
    public static final int Rx1 = 305;
    public static final int Ry1 = 285;
    public static final int Rx2 = 350;
    public static final int Ry2 = 315;
    
    //mouth 
    public static final int Mx1 = 265;
    public static final int My1 = 245;
    public static final int Mx2 = 280;
    
   // Hat Base
    public static final int hWidth = 55; 
    public static final int X_hat = 245;
    public static final int Y_hat = 210;
    public static final int hHeight = 7; 
    
    // Top Hat Rectangle
    public static final int tWidth = 45; 
    public static final int X_top = 250;
    public static final int Y_top = 170;
    public static final int tHeight = 40;
    
    
    public void init()
    {
        setBackground(Color.BLUE); 
    }
   
   public void paint (Graphics canvas)
   {
       //Sun 
       canvas.setColor(Color.YELLOW);
       canvas.fillOval(X_SUN, Y_SUN, SUN_DIAMETER, SUN_DIAMETER);
       
       
       canvas.drawString("Karen Toubbeh", 10, 15);
       
      
       
       //Gray Rect
       canvas.setColor(Color.DARK_GRAY);
       canvas.fillRect(X_RECT, Y_RECT, width, height );
       
       //Face 
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_FACE, Y_FACE, FACE_DIAMETER, FACE_DIAMETER);
       
       //middle body 
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_MIDDLE, Y_MIDDLE, MIDDLE_DIAMETER, MIDDLE_DIAMETER);
       
       
       //top button 
       canvas.setColor(Color.ORANGE);
       canvas.fillOval(X_tButton, Y_tButton, topB_DIAMETER, topB_DIAMETER);
       
       //top button 
       canvas.setColor(Color.ORANGE);
       canvas.fillOval(X_bButton, Y_bButton, bottomB_DIAMETER, bottomB_DIAMETER);
       
       //lower body
       canvas.setColor(Color.WHITE);
       canvas.fillOval(X_LOW, Y_LOW, LOW_DIAMETER, LOW_DIAMETER);
       
       //left eye
       canvas.setColor(Color.BLACK);
       canvas.fillOval(X_Leye, Y_Leye, Leye_DIAMETER, Leye_DIAMETER);
       
       //right eye 
       canvas.setColor(Color.BLACK);
       canvas.fillOval(X_Reye, Y_Reye, Reye_DIAMETER, Reye_DIAMETER);
       
       //left arm
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Lx1, Ly1, Lx2, Ly2 ); 
       
       //right arm
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Rx1, Ry1, Rx2, Ry2 ); 
       
       //Mouth
       canvas.setColor(Color.BLACK);
       canvas.drawLine(Mx1, My1, Mx2, My1 ); 
  
       //Hat Base
       canvas.setColor(Color.BLACK);
       canvas.fillRect(X_hat, Y_hat, hWidth, hHeight );
       
       //Top Hat
       canvas.setColor(Color.BLACK);
       canvas.fillRect(X_top, Y_top, tWidth, tHeight );
   }
   
   
}

                case 'K':
                case 'k':
                    myPet.poke();
                    break;
                case 'F':
                case 'f':
                    System.out.println("Feed how much? ");
                    int amtFood = input.nextInt();
                    myPet.feed(amtFood);
                    break;
                case 'E':
                case 'e':
                    System.out.println("Exercise how much? ");
                    int amtExercise = input.nextInt();
                    myPet.exercise(amtExercise);
                    break;
                case 'Q':
                case 'q':
                    keepGoing = false;
                    break;
                default:
                    System.out.println("Command not recognized.");
            }
        }
        
        System.out.println("Your pet expired :(");
    }
}

        Rectangle r1 = new Rectangle();
        

        r1.setWidth(3.0);
        r1.setLength(5.2);
            
        r1.printDimensions();
        
        
        Rectangle r2 = new Rectangle(2.6, 5.4);
        System.out.println();
        System.out.printf("Width: %.2f\n" , r2.getWidth()); 
        System.out.printf("Length: %.2f\n" , r2.getLength());
        System.out.println();
     
        
        
		System.out.printf("R1 Area: %.2f\n" , r1.getArea()); 
		System.out.printf("R1 Perimeter: %.2f\n" , r1.getPerimeter()); 
		
	
		
		System.out.printf("R2 Area: %.2f\n" , r2.getArea()); 
		System.out.printf("R2 Perimeter: %.2f\n" , r2.getPerimeter()); 
    }       
}
ring str)
    {
             
       if(str.length() >2)
    
       return str.substring(2)+str.substring(0, 2);
        
     
    }
    
    public static void sectionF(String str)
    {
        (str.length()/2) - 1
        
    
    }
    
    public static void sectionG(String str)
    {
        // Your code here...
        
             
    }
}

        
        
}
}

        
        
        
        

/**
 * Karen Toubbeh
 * CS 170 
 * March 20, 2017 
 */

public class Practice
{
    public static void main(String[] args)
    {
       int[] anArray = new int[10];
    for (int i = 0; i <anArray.length; i++)
        anArray[i] = 2 * i;
    for (int element : anArray)
        System.out.print(element + " ");
    System.out.println();
        
        
    }
}

    {
        //int[] a = {10,20,30,40,50};
        //int[] a = {45, 38, 27, 46, 81, 72, 56, 61, 20, 48, 76, 91, 57, 35, 78};
        int[] a = {45, 38, 27, 46, 81, 72, 56, 61, 20, 48, 76, 91, 57, 35, 800};
        int maxValue = a[0];
        int maxIndex = 0; 
        int sum = 0; 
        for (int idx = 1; idx < a.length; idx++)
        
        {
            if (a[idx] > maxValue)
            {
                maxValue = a[idx];
                maxIndex = idx; 
               
            }
            
            sum += a[idx];
        }
        System.out.println("The largest element is" +maxValue);
        System.out.println("The largest element is at index" +maxIndex);
        System.out.println("The sum of all elements is:" +sum);
     
        for (i % 2 == 0) 
        { 
            System.out.ptint(+sum);
        }
    }
}
		}
		
		System.out.println("\nSum of even numbers = " + sumE);
		
		i = x;
		System.out.print("Odd numbers: ");
		while (i<=y)
		{
			if (i%2==1)
			{
				sumO = sumO + i;
				System.out.print(i + " ");
			}
			i++;
		}
		System.out.println("\nSum of odd numbers = " + sumO);
}
}    

    
    
    
    
    
    
    
    
    
    
    
 * Exercise#01
 */
 
 public class MyFirstJavaProgram
  {
      public static void main (String[] args)
      {
          System.out.println("This is my first Java program!");
      }
      
  }
    
    
/*
 * Karen Toubbeh
 * CS A170
 * February 1,2017
 * 
 * Exercise#01
 */
 
 public class MyHousePrinterOneline
  {
      public static void main (String[] args)
      {
          System.out.println(" _____\n/_____\\\n|# _ #| \n|_| |_| ");
         
         
      }
      
  }
    
    
/*
 * Karen Toubbeh
 * CS A170
 * February 1,2017
 * 
 * Exercise#01
 */
 
 public class MySecondJavaProgram
  {
      public static void main (String[] args)
      {
          System.out.println("This is Karen's second Java program!");
      }
      /*
 * Karen Toubbeh
 * CS A170
 * Feburary 15, 2017
 * 
 * Excercise 03 
 */
import java.util.Scanner;
public class DayConverter
{
    public static void main(String[] args)
    {
        int day1 = 0;
        Scanner input = new Scanner(System.in);
        System.out.println("Enter a number of days: ");
        day1 = input.nextInt();
        int hours = 24 * day1;
        int mins = hours * 60;
        int secs = mins * 60;
        System.out.println(day1 + " days is " + hours + " hours or " + mins + " minutes or " + secs + " seconds");
    }
}
        
/*
 * Karen Toubbeh
 * CS A170
 * Feburary 15, 2017
 * 
 * Excercise 03 
 */
import java.util.Scanner;
public class HourConverter
{
    public static void main(String[] args)
    {
        int total = 0;
        Scanner input = new Scanner(System.in); 
        System.out.println("Enter a number of hours");
        total = input.nextInt();
        int weeks = total / 168;
        
        int total2 = total % 168;
        int days = total2 / 24;
        total2 = total % 24;
        int hours = total2 / 1; 
        
        System.out.println(total + " hours is " + weeks + " weeks, " + days + " days, and " + hours + " hours");
        
        
        
        
        
    }
}
        
/*
 * Karen Toubbeh
 * CS A170 
 * Feburary 15, 2017
 * 
 * Excercise 03
 */
import java.util.Scanner;
public class MathSkills
{
    public static void main(String[] args)
    {
        int N1 = 0;
        int N2 = 0;
        int N3 = 0;
        
        Scanner input = new Scanner(System.in);
        System.out.println("Enter THREE numbers and I will show you my math skills: ");
        N1 = input.nextInt();
        N2 = input.nextInt();
        N3 = input.nextInt();
        System.out.println("Check this out: ");
        int sum = (N1 + N2) - N3;
        int negN = N1 - N2 * N3;
        int Mult = (N1 - N2) * N3;
        int square = N1 * N1;
        System.out.println(N1 + " + " + N2 + " - "  + N3 + " = "  + sum);
        System.out.println(N1 + " - " + N2 + " * " + N3 + " = " + negN);
        System.out.println("(" +N1 + " - " + N2 + ")" + " * " + N3 + " = " + Mult);
        System.out.println( N1 +" Squared is " + square);
        
        
    }
}
/*
 * Karen Toubbeh
 * CS A170
 * February 15, 2017
 *
 * Exercise #03
 */
import java.util.Scanner;
public class NumberShape
{
    public static void main(String[] args)
  {
    Scanner keyboard = new Scanner(System.in);
    System.out.println("Enter a single digit number:/*
 * Karen Toubbeh
 * CS A170
 * February 25, 2017
 *
 * Exercise #08
 */


import java.text.DecimalFormat;
import java.util.Scanner;
 
public class FitnessPlanner_1
{
public static void main(String[] args) {
    
    
// Declarations
    Scanner input = new Scanner(System.in);

int calories= 47;

    //Ask the user for input
    System.out.println("Welcome to the Fitness Planner! This program will calculate how long you will need to exercise to burn off what you ate");
    
    System.out.println("Enter your weight in pounds: ");
    int weight = input.nextInt();
    
    System.out.println("Enter the number of chicken nuggets you ate: ");
    int chickenNuggets = input.nextInt();
    
    System.out.println("Enter your average WALKING speed in mph(3 is common, 20-min/mile pace): ");
    int walkingSpeed = input.nextInt();
    
    System.out.println("Enter your average RUNNING speed in mph(6 is common, a 10-min/mile pace): ");
    int runningSpeed = input.nextInt();


    double vWalking = (2.68224 * walkingSpeed + 3.5);
	double vRunning = (5.36448 * runningSpeed + 3.5);
		
	double cbrWalking = ((2.268 * Math.pow(10,-3))* vWalking * weight);
	double cbrRunning = ((2.268 * Math.pow(10,-3))* vRunning * weight);

    int totalCalories = chickenNuggets * calories;
    double resultWalking = totalCalories / cbrWalking;
    double resultRunning = totalCalories / cbrRunning;
    
    DecimalFormat zero = new DecimalFormat("0");
    
        System.out.println("You need to walk for " + zero.format(resultWalking) + " minutes to burn off the 20 chicken nuggets you ate.");
        System.out.println("You need to run for " + zero.format(resultRunning) + " minutes to burn off the 20 chicken nuggets you ate.");





    }
}




/*
 * Karen Toubbeh
 * CS A170
 * February 25, 2017 
 *
 * Exercise #08
 */


import java.text.DecimalFormat;
import java.util.Scanner;
 
public class FitnessPlanner_2
{
public static void main(String[] args) {
    
    
// Declarations
    Scanner input = new Scanner(System.in);

int calories= 47;

    //Ask the user for input
    System.out.println("Welcome to the Fitness Planner! This program will calculate how long you will need to exercise to burn off what you ate");
    
    System.out.println("Enter your weight in pounds: ");
    int weight = input.nextInt();
    
    System.out.println("Enter the number of chicken nuggets you ate: ");
    int chickenNuggets = input.nextInt();
    
    System.out.println("Do you prefer walking or running (W or R)? ");
    String userInput = input.next();

            int totalCalories = chickenNuggets * calories;
    DecimalFormat zero = new DecimalFormat("0");

        
        
    if(userInput.equalsIgnoreCase("w"))
    {
        System.out.println("Enter your average WALKING speed in mph(3 is common, 20-min/mile pace): ");
        int walkingSpeed = input.nextInt();
        
            double vWalking = (2.68224 * walkingSpeed + 3.5);
            	double cbrWalking = ((2.268 * Math.pow(10,-3))* vWalking * weight);
            	    double resultWalking = totalCalories / cbrWalking;
        System.out.println("You need to walk for " + zero.format(resultWalking) + " minutes to burn off the " + chickenNuggets +" chicken nuggets you ate.");



        

    }
    
    
    else if(userInput.equalsIgnoreCase("r"))
    {
        System.out.println("Enter your average RUNNING speed in mph(6 is common, a 10-min/mile pace): ");
        int runningSpeed = input.nextInt();
        double vRunning = (5.36448 * runningSpeed + 3.5);
		
    	double cbrRunning = ((2.268 * Math.pow(10,-3))* vRunning * weight);
    	    double resultRunning = totalCalories / cbrRunning;
        System.out.println("You need to run for " + zero.format(resultRunning) + " minutes to burn off the " + chickenNuggets +  " chicken nuggets you ate.");
        

    }


	

    
    





    }
}




/*
 * Karen Toubbeh
 * CS A170
 * February 25, 2017
 *
 * Exercise #08
 */

import java.text.DecimalFormat;
import java.util.Scanner;
 
public class FitnessPlanner_3
{
public static void main(String[] args) {
    
    
// Declarations
    Scanner input = new Scanner(System.in);

int calories= 47;

    //Ask the user for input
    System.out.println("Welcome to the Fitness Planner! This program will calculate how long you will need to exercise to burn off what you ate");
    
    System.out.println("Enter your weight in pounds: ");
    int weight = input.nextInt();
    
    
    System.out.println("Do you prefer walking or running (W or R)? ");
    String userInput = input.next();

    //int totalCalories = chickenNuggets * calories;
    DecimalFormat zero = new DecimalFormat("0");

        
        
    if(userInput.equalsIgnoreCase("w"))
    {
        System.out.println("Enter your average WALKING speed in mph(3 is common, 20-min/mile pace): ");
        int walkingSpeed = input.nextInt();
        
        System.out.println("How many minutes will you walk? ");
        int minutesWalk = input.nextInt();
        
            double vWalking = (2.68224 * walkingSpeed + 3.5);
            	double cbrWalking = ((2.268 * Math.pow(10,-3))* vWalking * weight);
            	    
            	    
            
    	    double chickenNuggets = (cbrWalking*minutesWalk)/calories;
    	    
    	    double totalCalories = chickenNuggets * calories;
    	    double resultWalking = totalCalories / cbrWalking;
            	    
            	    
            	    
            	    //HERE
            	    
            	    
            	    
        System.out.println("Congratulations, you are allowed to eat " + (int)chickenNuggets + " chicken nuggets.");
        System.out.println("You will burn off " + (int)totalCalories + "calories later.");


        

    }
    
    
    else if(userInput.equalsIgnoreCase("r"))
    {
        System.out.println("Enter your average RUNNING speed in mph(6 is common, a 10-min/mile pace): ");
        int runningSpeed = input.nextInt();
        
        System.out.println("How many minutes will you Run? ");
        int minutesRunning = input.nextInt();
        

        
        double vRunning = (5.36448 * runningSpeed + 3.5);
		
    	double cbrRunning = ((2.268 * Math.pow(10,-3))* vRunning * weight);
    	    
    	    double chickenNuggets = (cbrRunning*minutesRunning)/calories;
    	    
    	    double totalCalories = chickenNuggets * calories;
    	    double resultRunning = totalCalories / cbrRunning;

    	    
          System.out.println("Congratulations, you are allowed to eat " + ((int)chickenNuggets) + " chicken nuggets.");
        System.out.println(" You will burn off " + (int)totalCalories + " calories later.");
    }


	

    
    





    }
}



");
    int myNum; 
    myNum = keyboard.nextInt();
    System.out.println (""+myNum+""+myNum+" "+myNum+" "+myNum+""+myNum+"");
    System.out.println (" "+myNum+""+myNum+" "+myNum+""+myNum+"");
    System.out.println ("  "+myNum+" "+myNum+"");
    System.out.println ("   "+myNum+"");
    
    
  }
}
  }
    
    
    
    
