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

BREAKING DOWN THE ANATOMY OF A METHOD
1. public (access modifier): public allows parts of the program outside of the class to call on it. If it was private, then only that specific class could call on it, which would make it pretty useless.

2. stati: in a real world example, the recipe can be used to make whatever, but it doesn't always have to be a cake?"
"so if i understand this, then static means the program will pull from the original class, which applies to the broadest use case, instead of a potentially specific use case?

3. void: This is the return type. It means that your program will run without having to return anything, like a string.

4. main (Method Name): it represents what I want the code to do, which is in the name.

5. (String[] args): These are the parameters. Having nothing between the parentheses means that the program does not require any input in order to run. But if there is something between them, then you can run commands that include that.

GETTING A METHOD TO RETURN SOMETHING
Coursera uses a comparison to giving your friend a treasure map. If you use 'void', it's like you giving them the map, and them giving you nothing in return for finding it.
So, breaking down the steps helps us figure out where exactly we need to prompt Java to giving us a return:
1. Following the Map (Non-Returning Methods):
- To keep in line with the example already given, say you add instructions that say digHere. This will make Java look in this spot
for treasure, but that doesn't mean it will find anything of value. In the programming world, such methods might rearrange things internally, like gathering ingredients for a recipe. However, they do not provide a specific answer or a piece of data, like the final delicious meal.

2. Treasure Trove Methods (Returning a Value):
- This is like following clues on a treasure map. By giving Java certain perameters to look for, you're giving it context to look for exactly what you want it to, leading it closer to providing the return you desire.

Putting Both Parts Together
The non-returning methods help you to progress through the treasure hunt. Just like following instructions leads us to different locations, these methods can move a program through different steps, even if they don’t directly provide the result.

The returning methods can return different types of treasures, depending on the kind of clue they unearth. They might return a simple arrow pointing to the following location, a short riddle to solve, or even a more complex drawing like the detailed map of the next area. The critical point is that they bring back something valuable that helps you to progress further in your treasure hunt. 

### Passing Arguments to Methods




































# DAILY TRACKING SUMMARY
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

## April 30, 2025
### Reading: Writing Method Signatures
One important thing to remember about methods in Java is that they have 'signatures' that identify what they are, similar
to how we use signatures when setting up bank accounts or writing checks, it's a way to verify that we are the one initiating the action.

### Main method
```java
public static void main(String[] args) {
// instructions to be performed
}
```
Breaking each part down:
- public: is like stating that “anyone can follow these steps.”
Hello, I am accessible to anyone!
Even your friend can read me.
static: is like saying, “These steps are always the same for this device.”

You can operate many similar devices using these exact instructions.
The basic instruction set is shared among all the devices.

- void: means this section does not give you anything back directly, unlike the > (greater than) operator that always returns a result in either true or false.

Reading the booklet is an action, but it does not prepare your device for use. There are more steps to follow.

- main: tells you what it does: Just like the booklet's first page might say “Getting Started,” the word main says, “This is the most important section for getting the program running.”

- (String[] args): is similar to saying, “This section might take some optional instructions or inputs later on, but they’re not needed to get started yet.”

Since it is an array, it can be empty!

Set of curly braces {} - contains all the instructions to be performed when the program starts.

Here is how it works explained simply, for me:
- What it does: Start the program (similar to “Getting Started”).
- How to use it: Just call “main” without any extra information.
-What to expect: It might not give the result directly, but it sets the program in motion.
This is what the signature of every method tells you!

Understanding the technical jargon, important for down the road:
- The keyword public is called an access modifier because it makes the method available to anyone who wants to use it
- The keyword static is like a sharing mechanism because it creates a single version of a method that all parts of the program can access. If you don’t want to share your method, you can skip it.
- The keyword void is a return type because it indicates that the method does not give something in return for being called
 -The keyword main is the method name. That is how Java recognizes the starting point of a program. For the methods you create, it can be a verb signifying the purpose of the method
- The (String[] args), such as the parentheses (empty or not empty), is called the parameter list because this is where you provide some input or information to the method. You can also offer multiple inputs, which is why it is called a list. Every time you use a print statement, you are providing parameters to a method, System.out.println(parameters);.


## May 3, 2025
I watched a video about passing arguments to methods, and part of that was building a "superhero fighting project" type thing. So I'll upload that separately for viewing.


## May 4, 2025
First thing on the list today is completing a graded lab called Writing Methods. It uses code I wrote in a previous lab and I'll be repurposing it to reinforce how you can use methods to change the behavior of your code. Will upload it when I finish.


## May 12, 2025
### Classes and Objects
Today started with a video about classes and objects. It explained what each is, and what they're used for, using the previous superhero example.
Classes- Like explained last week, a class is a blueprint for the program that defines the characteristics and methods of objects in the code, thus making it more organized and easier to read.
Objects- These are specific instances of classes, which are created through a process of instantiation, which is a fancy way of desribing giving life to the object.

Instantiation: This allows the programmer to create new instances of a class while referencing the original. For example, say there is a class called cat, but I want to create an instance of that class that applies to my cat, Roo. I would use this concept to create an instance of the cat class, new cat ("Roo')

Up next is a lab called 'Creating Classes'. SEE REPO FOR WORK














