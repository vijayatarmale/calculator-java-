# calculator-java-
import java.util.Scanner;

public class SimpleCalculator {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        
        System.out.println("Simple Calculator");
        System.out.print("Enter the first number: ");
        double num1 = input.nextDouble();
        
        System.out.print("Enter the operator (+ or -): ");
        char operator = input.next().charAt(0);
        
        System.out.print("Enter the second number: ");
        double num2 = input.nextDouble();
        
        double result = 0.0;
        
        if (operator == '+') {
            result = num1 + num2;
        } else if (operator == '-') {
            result = num1 - num2;
        } else {
            System.out.println("Invalid operator. Please use + or -.");
            return;
        }
        
        System.out.println("Result: " + result);
        
        input.close();
    }
}

