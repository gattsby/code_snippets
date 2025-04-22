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
A good example for this would be if you were building a program that makes a robot clean the house. You would want to label each room you want it to clean in a numbered list, with the option to input a number between 1 and however many rooms you have chosen to include. From there use a switch method:

```
switch (cleaningOption) {
  case 1:
    System.out.println("Cleaned attic");
    break;

  // remember to add breaks so that the code will function as intended, otherwise it will fallthrough
```

