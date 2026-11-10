# Regex-Activity


// Name: Trexie Joy Dubria
// Section: BSIT-2B

import java.util.*;
import java.util.regex.*;

public class Regex {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while (true) {

            System.out.print("Enter a string: ");
            String input = sc.nextLine();
            System.out.println();

            System.out.println("Only digits: " +
                    Pattern.matches("[0-9]+", input));

            System.out.println("Only letters: " +
                    input.matches("(?i)[a-z]+"));

            System.out.println("Letters and numbers: " +
                    (input.matches("(?i).*[a-z].*") &&
                     input.matches(".*[0-9].*")));

            System.out.println("Starts with Java: " +
                    input.matches("(?i)^Java.*"));

            System.out.println("Ends with .com: " +
                    input.matches("(?i).*\\.com$"));

            System.out.println("Exactly 5 digits: " +
                    input.matches("[0-9]{5}"));

            System.out.println("At least 8 characters: " +
                    input.matches(".{8,}"));

            Pattern pattern = Pattern.compile("\\s");
            Matcher matcher = pattern.matcher(input);

            System.out.println("Contains whitespace: " +
                    matcher.find());

            System.out.println();
        }

    }
}

// Name: Ranil Delalamon
// Section: BSIT-2B

import java.util.*;
import java.util.regex.*;

public class Regex {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while (true) {

            System.out.print("Enter a string: ");
            String input = sc.nextLine();
            System.out.println();

            System.out.println("Only digits: " +
                    Pattern.matches("[0-9]+", input));

            System.out.println("Only letters: " +
                    input.matches("(?i)[a-z]+"));

            System.out.println("Letters and numbers: " +
                    (input.matches("(?i).*[a-z].*") &&
                     input.matches(".*[0-9].*")));

            System.out.println("Starts with Java: " +
                    input.matches("(?i)^Java.*"));

            System.out.println("Ends with .com: " +
                    input.matches("(?i).*\\.com$"));

            System.out.println("Exactly 5 digits: " +
                    input.matches("[0-9]{5}"));

            System.out.println("At least 8 characters: " +
                    input.matches(".{8,}"));

            Pattern pattern = Pattern.compile("\\s");
            Matcher matcher = pattern.matcher(input);

            System.out.println("Contains whitespace: " +
                    matcher.find());

            System.out.println();
        }

    }
}
