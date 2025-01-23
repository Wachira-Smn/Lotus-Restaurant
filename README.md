# oop-2-assingment
// Source code is decompiled from a .class file using FernFlower decompiler.
import java.util.Scanner;

public class Bonus {
   public Bonus() {
   }

   public static void main(String[] var0) {
      Scanner var1 = new Scanner(System.in);
      System.out.println("Enter the number of years of service:");
      int var2 = var1.nextInt();
      System.out.println("Enter the salary:");
      double var3 = var1.nextDouble();
      double var5 = calculateBonus(var2, var3);
      System.out.println("The bonus is: " + var5);
   }

   public static double calculateBonus(int var0, double var1) {
      double var3;
      if (var0 >= 10) {
         var3 = var1 * 0.12;
      } else if (var0 >= 6) {
         var3 = var1 * 0.05;
      } else {
         var3 = var1 * 0.02;
      }

      return var3;
   }
}
