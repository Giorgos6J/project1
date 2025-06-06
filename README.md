import java.util.Scanner;

public class Main { public static void main(String[] args) { Scanner scanner = new Scanner(System.in);

    System.out.println("Enter your name:");
    String name = scanner.nextLine();

    System.out.println("Enter your second name:");
    String secondName = scanner.nextLine();

    System.out.printf("Hello user %s %s\n", secondName, name);

    int n;
    System.out.println("Input key pass (type 0 to exit):");

    while ((n = scanner.nextInt()) != 0) {
        System.out.println("Give task number:");
        int n1 = scanner.nextInt();

        if (n1 == 10) {
            int a1 = scanner.nextInt();
            int a2 = scanner.nextInt();

            System.out.println("Sum: " + (a1 + a2));
            System.out.println("Difference: " + (a1 - a2));
            System.out.println("Modulo: " + (a1 % a2));
            System.out.println("Product: " + (a1 * a2));
        }

        if (n1 == 20) {
            System.out.println("Give height:");
            int h = scanner.nextInt();
            System.out.println("Give side a length:");
            int a = scanner.nextInt();
            System.out.println("Give side b length:");
            int b = scanner.nextInt();
            System.out.println("Give side c length:");
            int c = scanner.nextInt();

            if (a == b && b == c) {
                System.out.println("Equilateral triangle");
            } else if (a == b || b == c || a == c) {
                System.out.println("Isosceles triangle");
            } else {
                System.out.println("Scalene triangle");
            }

            int area = (h * a) / 2;
            int perimeter = a + b + c;
            System.out.println("Area: " + area);
            System.out.println("Perimeter: " + perimeter);
        }

        if (n1 == 30) {
            int s1 = scanner.nextInt();
            System.out.println("Give side a length:");
            int s2 = scanner.nextInt();

            if (s1 == s2) {
                System.out.println("Square");
            } else {
                System.out.println("Rectangle");
            }

            System.out.println("Area: " + (s1 * s2));
            System.out.println("Perimeter: " + (2 * (s1 + s2)));
        }

        if (n1 == 40) {
            int radius = scanner.nextInt();
            double diameter = 2 * radius;
            double area = Math.PI * radius * radius;
            double circumference = 2 * Math.PI * radius;

            System.out.println("Diameter: " + diameter);
            System.out.println("Area: " + area);
            System.out.println("Circumference: " + circumference);
        }

        if (n1 == 50) {
            int s1 = scanner.nextInt();
            System.out.println("Give side s2:");
            int s2 = scanner.nextInt();

            double pow1 = Math.pow(s1, s2);
            double pow2 = Math.pow(s2, s1);

            int diff = s1 - s2;
            if (diff > 0) {
                double sqrt = Math.sqrt(diff);
                System.out.println("Square root of difference: " + sqrt);
            }
        }

        if (n1 == 60) {
            int number = scanner.nextInt();
            for (int i = 1; i <= 10; i++) {
                System.out.printf("%d * %d = %d\n", number, i, number * i);
            }
        }

        if (n1 == 70) {
            int number = scanner.nextInt();
            if (number > 100) {
                int lastDigit = number % 10;
                System.out.println("Last digit: " + lastDigit);
            }
        }

        if (n1 == 80) {
            System.out.println("Enter a number:");
            int number = scanner.nextInt();
            System.out.println("Factors:");
            for (int i = 1; i <= number; i++) {
                if (number % i == 0) {
                    System.out.print(i + " ");
                }
            }
            System.out.println();
        }
    }

    System.out.println("Goodbye " + name + " " + secondName);
    scanner.close();
}
}
