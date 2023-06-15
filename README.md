
Import java.util.Scanner;



Public class UserDetails {

    Public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);



        System.out.print(“Enter your surname: “);

        String surname = scanner.nextLine();



        System.out.print(“Enter your age: “);

        Int age = scanner.nextInt();



        printSurnameDetails(surname);

        printAgeDetails(age);



        scanner.close();

    }



    // Method to print the number of characters in the surname

    Public static void printSurnameDetails(String surname) {

        Int length = calculateSurnameLength(surname);

        System.out.println(“Number of characters in your surname: “ + length);

    }



    // Method to calculate the number of characters in the surname

    Public static int calculateSurnameLength(String surname) {

        Return surname.length();

    }



    // Method to print whether the age is even or odd

    Public static void printAgeDetails(int age) {

        String type = determineAgeType(age);

        System.out.println(“Your age is “ + type + “.”);

    }



    // Method to determine whether the age is even or odd

    Public static String determineAgeType(int age) {

        Return (age % 2 == 0) ? “even” : “odd”;

    }

}
