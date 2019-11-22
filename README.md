# School-Programming4
The fourth programming project for my class

package Chapter6PPMatthewRoberts;

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
