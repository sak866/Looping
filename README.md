# LoopingWrite a program to print the numbers from 10 to 50 using for loop/while loop.
public class Forloop{
    public static void Forloop(String[] args) {
        for (int i = 10; i <= 50; i++) {
            System.out.println(i);
        }
    }
}
public class Whileloop {
    public static void Whileloop(String[] args) {
        int i = 10;
        while (i <= 50) {
            System.out.println(i);
            i++;
        }
    }
}
2.Write a program that find a given number is negative or positive. Input=123

Output Positive

Input — 100

Output-Negative

import java.util.Scanner;

public class  PositiveOrNegative{
    public static void PositiveOrNegative(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = input.nextInt();

        if (number > 0) {
            System.out.println("Positive");
        } else if (number < 0) {
            System.out.println("Negative");
        } else {
            System.out.println("Zero");
        }
    }
}
3.Write down the program to reverse the given number using loops.

Input = 876

Output=678

mport java.util.Scanner;

public class ReverseNumber {
    public static void ReverseNumber(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = input.nextInt();
        int reversed = 0;

        while (number != 0) {
            int digit = number % 10;       
            reversed = reversed * 10 + digit; 
            number /= 10;                  
        }

        System.out.println("Reversed number: " + reversed);
    }
}
4. Write a java program to Find the smallest number among three numbers

import java.util.Scanner;

public class ThreeNumbers {
    public static void ThreeNumbers(String[] args) {
        Scanner input = new Scanner(System.in);

        // Take input for three numbers
        System.out.print("Enter first number: ");
        int num1 = input.nextInt();

        System.out.print("Enter second number: ");
        int num2 = input.nextInt();

        System.out.print("Enter third number: ");
        int num3 = input.nextInt();

        int smallest;

    
        if (num1 <= num2 && num1 <= num3) {
            smallest = num1;
        } else if (num2 <= num1 && num2 <= num3) {
            smallest = num2;
        } else {
            smallest = num3;
        }

        System.out.println("The smallest number is: " + smallest);
    }
}

//Enter first number: 25
//Enter second number: 12
//Enter third number: 30
5. Write a Java program that takes the purchase amount as input and calculates the final payable amount after applying the discount

1. If the purchase amount is less than 500, no discount is applied.

2. If the purchase amount is between 500 and 1000, a 10% discount is applied 3. If the purchase amount is greater than 1000 a 20% discount is applied

import java.util.Scanner;

public class Discounted {
    public static void Discounted(String[] args) {
        Scanner input = new Scanner(System.in);

       
        System.out.print("Enter the purchase amount: ");
        double amount = input.nextDouble();
        double discount = 0;

        
        if (amount >= 500 && amount <= 1000) {
            discount = amount * 0.10;  // 10% discount
        } else if (amount > 1000) {
            discount = amount * 0.20;  // 20% discount
        }

        double finalAmount = amount - discount;

        // Output results
        System.out.println("Discount applied: ₹" + discount);
        System.out.println("Final payable amount: ₹" + finalAmount);
    }
}


// Enter the purchase amount: 450
6. Write a java program to print bellowed patterni and j and k>5

55555

54444

54333

54322

54321

public class Pattern {
    public static void Pattern(String[] args) {
      
        for (int i = 1; i <= 5; i++) {
            
            for (int j = 5; j >= 1; j--) {
                if (j > i) {
                    System.out.print(j);
                } else {
                    System.out.print(i);
                }
            }
            
            System.out.println();
        }
    }
}


