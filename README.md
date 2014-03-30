GUESS-USING-WHILE
=================

GUESSING NUMBER USING "WHILE"


// By   Reina Olarte
// Guessing Number Ussing WHILE

import java.util.Scanner;
// imports the scanner class
import java.util.Random
;// imports the random class

public class WhileLoop
{
	public static void main( String[]args)
	{

		//Create the Scanner to input the number
		Scanner input = new Scanner(System.in);
		//Create the Random number
		Random randomNumber = new Random();

		int i =0;

		while( i<3)
		{

		//Declaring the variables
		int UserNumber;
		int computerNumber;

		computerNumber = 0 + (int)(Math.random() *10);


		System.out.println("Welcome to the Guessing game\nPlease enter a digit from 0 to 10:");
		UserNumber = input.nextInt();

		if (computerNumber == UserNumber)
		{
			System.out.println("You Guessed the right number");
			System.out.printf("Your number %d, Random number %d\n\n" , UserNumber, computerNumber);
		}

		else
			{
				if (computerNumber < UserNumber)
				{
					System.out.println("You Guessed to High");
					System.out.printf("Your number %d, Random number %d\n\n" , UserNumber, computerNumber);
				}
				else
				{	System.out.println("You Guessed to Low");
				System.out.printf("Your number %d, Random number %d\n\n" , UserNumber, computerNumber);
				}	
			}
		i++;

		}   //end of while loop
	}   //End main

}   //End class
