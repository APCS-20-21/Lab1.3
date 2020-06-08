# Lab 1.3 Reading Input with Scanner

## Instructions

You will write a program that asks the user some questions, processes that information, and outputs responses.

All of the code you write will go inside the main method of the ScanningInput class. There are two helpful comments to identify where your code should go. Do not write code anywhere else in the file!

```
public class ScanningInput
{
  public static void main(String[] args)
  {
    // WRITE YOUR CODE BELOW THIS LINE


    // WRITE YOUR CODE ABOVE THIS LINE
  }
}
```

In order to read input from a user you need to use a Scanner object. Before you can use a Scanner object you must *instantiate* it with the following statement:

```
Scanner user = new Scanner(System.in);
```

Once you have instantiated a Scanner object and stored it in a variable (in this example, the variable name is *user*) you can use that object to get data from the user using the following statements:

```
String word = user.next();
int number = user.nextInt();
double decimal = user.nextDouble();
```

You should name your variables something appropriately descriptive of the data the user is inputting. In this example above the variables are named *word*, *number*, and *decimal*, but if you asked the user to input how tall they are you might name that variable *height*.

When you want to output text to the user, you will use the System.out.println method like this:

```
System.out.println("Computer Science!");
```

And remember you can use concatenation to combine two strings. You can even combine string literals and string variables!

```
String a = "Science";
String b = "Computer " + a + "!";
```

Your program will ask the following questions exactly as presented, and output the following responses exactly as presented.

### Question 1

```
What is your first name?
```

The user will enter a single word (no spaces). Assume they typed the name *Justin*, then your program will output the response:

```
Hello Justin
```

You will need to store the user's response in a variable and use concatenation to generate this response. This is the process you will follow to generate all the responses.

### Question 2

```
What year were you born?
```

The user will enter a 4 digit number. Assume they typed the number *2005*, then your program will output the response:

```
Awesome, so you are about 15 years old!
```

You will need to subtract the number they enter from 2020 to determine their age. 2020 -2005 = 15.

### Question 3

```
Enter a number greater than 1000.
```

The user will enter a whole number that is greater than 1000 (so it has at least 4 digits in it). Assume they typed the number *8675*, then your program will output the response:

```
The ones digit of 8675 is 5
If you remove the ones digit, you get 867
```

You will have to do some math to isolate the ones digit from the number and to remove the ones digit from the number. Thing about the different math operators we learned about ( + - * / % ). Which of these operators can be used to isolate the ones digit of a number and which one can be used to remove the ones digit of a number?

Hint: our number system is a *base-10*. What does that mean? How does that help you solve this problem?

### Question 4

```
Enter a number with a decimal place.
```

The user will enter a number that includes a decimal place. Assume they typed the number *3.141592*, then your program will output the response:

```
The truncated version of 3.141592 is 3
```

Since the user will be entering a double value, you will have to convert that into an int value to truncate it!

## Example

User input will be denoted with square-brackets in this example. But the user would not actually be typing the square-brackets and you would not actually see them in the output. They are only being used in this example to distinguish between text that is typed by the user and text that is output by the program.

```
What is your first name?
[Justin]
Hello Justin
What year were you born?
[1776]
Awesome, so you are about 244 years old!
Enter a number greater than 1000.
[1234]
The ones digit of 1234 is 4
If you remove the ones digit, you get 123
Enter a number with a decimal place.
[1234.5678]
The truncated version of 1234.5678 is 1234
```

Double check your program's output to make sure it has all the periods and question marks and correct spacing!

## Testing

Start small, and test as you go. Write code so that your program asks the first question. Then run your program and test it. Then, make your program output the response. Once you are happy with the result, move on to the next question.

Basically, you should save, compile, and test your program after every 1 or 2 lines of code that you write!

## Grading

This lab will be automatically graded by comparing the output of the program to the expected output. Your output must match the expected output exactly. That means spelling, spaces, line breaks, and punctuation must all match exactly. If your output is missing a . then it will not match the expected output and will be marked as *incorrect*.

Your output must match the expected output exactly to receive credit for this lab. Use the example as a guide to make sure your output is correct.

## Turning it in

When you have finished this lab, upload it to [MrMayCS.com/turnitin](http://mrmaycs.com/turnitin)
