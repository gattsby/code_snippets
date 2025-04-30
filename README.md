# code_snippets
a collection of useful snippets that I imagine I'll need to reference a lot


# Java `while` Loop

The `while` loop runs as long as the condition is true. It's useful when you don’t know ahead of time how many times something needs to run.

## 🔄 Basic Syntax

```java
while (condition) {
    // code block to be executed
}
```
When working with a while loop that you want to loop indefinitely until the user decides to exit the code, use a boolean (true/false) variable.
### While loops run while the boolean condition is true, to end one, add a false condition so the program knows when to stop

A good example for this would be if you were building a program designed to command a robot clean the house. You would want to label each room you want it to clean in a numbered list, with the option to input a number between 1 and however many rooms you have chosen to include. From there use a switch method:

```java
switch (cleaningOption) {
  case 1:
    System.out.println("Cleaned attic");
    break;
}
    // remember to add breaks so that the code will function as intended, otherwise it will fallthrough
```

Ex.

```java
public class Main {
    public static void main)String{} args) {

        int totalTrashInRoom = 0;

        do {
            System.out.println("I will take out some trash. ");
        } while( totalTrashInRoom > 0);
    }
}
```

### while loops are best used for when boolean conditions are true and repetitive menus. A variation of the while loop is the do-while loop

# Implementing while loops

A while loop lets you execute a block of code repeatedly while a certain condition within that block is true. Making it useful for programs you want to run until a specific condition is met (like cleaning the house)
Another useful example would be to use this for a counting app.

```java
public class SimpleCounter {
    public static void main(String[] args) {
        int count = 1;  // Start with 1

        while (count <= 5) {
            System.out.println("Count is: " + count);
            count++;  // Increase count by 1
        }
    }
}
```
the output for this block should thenn show the count going up by 1 interval (count++) until it reaches the number 5, at which point the code specified using the while loop to stop counting when the value of the condition was less than or equal to 5. ( while (count <= 5) )

## Example 2: Guessing Game
While loops can also be used to create simple games, like a guessing game. The idea is simple:
- The computer has a secret number.

- The player will keep guessing what that number is from 1 to 9.

- After each guess, the computer will tell you whether your guess was correct or not.

- If your guess is wrong, the loop will continue, giving you another chance to guess.

- If your guess is right, the loop will stop, and the computer will congratulate you.
### Why a while loop is best for this
It allows for an indefinite number of guesses until the user guesses correctly until they guess the correct answer.
```java
import java.util.Scanner;

public class GuessingGame {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // Scanner to read user input
        int secretNumber = 7;  // The secret number to guess
        int userGuess = 0;  // Variable to store the user's guess, initialized with 0

        // While loop that keeps running until the correct guess
        while () { // TODO 1 - Write the exit condition
            System.out.print("Guess the number from 1 to 9: ");
            // TODO 2: GET input from user 

            if (userGuess != secretNumber) {
                System.out.println("Wrong guess, try again!");
            }
        }

        // TODO 3: Congratulate the user once they guess correctly
    }
}
```
According to this lesson, it would seem that the 'scanner' function can only be run in IntelliJ, so I might have to look into that.






### MODULE 3: Using Methods
Why use methods? It allows you to break down a larger task into smaller, more manageable ones. Like making a sandwich for example. Instead of having to tackle the entire process of 
making a sandwich, why not break it down into smaller, easier to complete steps, and combine all 3 to make the whole system work. A great example of a method that I've seen and didn't
realize is the "MAI" method:

```java
        public class Main {
        public static void (Strings[] args( {
    }
}
```
Methods also have a pair of curly braces used to write the instructions for accomplishing the task. The main thing to remember about when using these is they are placed *outside* of the main class.





























### DAILY TRACKING SUMMARY
## Week of April 30, 2025

🧠 **What I focused on:**
- Conditionals and basic loops
- Reviewing note structure and making it easier to skim

📈 **Wins:**
- Showed up even when I was low-energy
- Pushed 3+ commits to repo

💡 **Struggles:**
- Felt mentally worn out most days
- Had trouble focusing beyond 10 mins

🔁 **Next Week Goal:**
- Keep 10–20 min habit going
- Try 1 hands-on mini coding task (if energy allows)









