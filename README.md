# School-Programming4
The fourth programming project for my class

package Chapter6PPMatthewRoberts;
/* Matthew Roberts
 * 11/08/2019
 * Project 6
 * Extra Credit:
 * Project Description:  
 * 1) Get user's full name with one statement.
 * 2) Based on the number of characters, ask the user to to enter that many numbers and add the total.
 * 3) Display the appropriately versed and formatted.
 

 */

import java.util.Scanner;

public class Chapter6PPMatthewRoberts {

	public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		String name="full name", quit = "quit";
		int number, total;
		
		while (true ) {
			total=0;
			
		System.out.println("Please enter your name: ");
		name = scan.nextLine();
		if (name.equalsIgnoreCase(quit))
			break;	
		final int END = (name.length());
		System.out.println("Please enter " + END + " numbers and the total will be calculated: ");
		for (int i = 0; i < END; i++) {
			number = scan.nextInt();
			total += number;}
		
		
		System.out.println("Good day, " + name + " You have entered " + END + " numbers." +
		" The total of all the numbers is  " + total);
		scan.nextLine();
		
		}
		
		System.out.println("Thank you for using the system. Come back soon.");
		
		

	}

}
