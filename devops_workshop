package com.Project.Maven_app;

public class App {
    public static void main(String[] args) {
        if (args.length != 3) {
            System.out.println("Usage: java CommandLineCalculator <num1> <operator> <num2>");
            System.out.println("Example: java CommandLineCalculator 10 + 5");
            return;
        }

        try {
            double num1 = Double.parseDouble(args[0]);
            String operator = args[1];
            double num2 = Double.parseDouble(args[2]);
            double result = 0;

            switch (operator) {
                case "+":
                    result = num1 + num2;
                    break;
                case "-":
                    result = num1 - num2;
                    break;
                case "*":
                    result = num1 * num2;
                    break;
                case "/":
                    if (num2 == 0) {
                        System.out.println("Error: Division by zero is not allowed.");
                        return;
                    }
                    result = num1 / num2;
                    break;
                default:
                    System.out.println("Error: Unsupported operator. Use +, -, *, or /.");
                    return;
            }

            System.out.printf("Result: %.2f %s %.2f = %.2f%n", num1, operator, num2, result);
        } catch (NumberFormatException e) {
            System.out.println("Error: Invalid number format. Please provide valid numbers.");
        }
    }
}
