// Importing the Scanner class to allow user input
import java.util.Scanner;

public class Bonus {

   // Constructor for the Bonus class (not used in this case)
   public Bonus() {
   }

   // Main method: the entry point of the program
   public static void main(String[] var0) {
      // Create a Scanner object to read input from the user
      Scanner var1 = new Scanner(System.in);

      // Prompt the user to enter the number of years of service
      System.out.println("Enter the number of years of service:");
      int var2 = var1.nextInt(); // Store the user's input as an integer (years of service)

      // Prompt the user to enter their salary
      System.out.println("Enter the salary:");
      double var3 = var1.nextDouble(); // Store the user's input as a double (salary)

      // Call the calculateBonus method to compute the bonus based on years of service and salary
      double var5 = calculateBonus(var2, var3);

      // Print the calculated bonus to the user
      System.out.println("The bonus is: " + var5);
   }

   // Method to calculate the bonus based on years of service and salary
   public static double calculateBonus(int var0, double var1) {
      double var3; // Variable to store the calculated bonus

      // Check if the number of years of service is 10 or more
      if (var0 >= 10) {
         var3 = var1 * 0.12; // Bonus is 12% of the salary
      } 
      // Check if the number of years of service is between 6 and 9 (inclusive)
      else if (var0 >= 6) {
         var3 = var1 * 0.05; // Bonus is 5% of the salary
      } 
      // If the number of years of service is less than 6
      else {
         var3 = var1 * 0.02; // Bonus is 2% of the salary
      }

      // Return the calculated bonus
      return var3;
   }
}
