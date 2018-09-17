# Javastuff

/*
 * Karen Toubbeh
 * CS A170
 * February 1,2017
 * 
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
    
    
    
    
