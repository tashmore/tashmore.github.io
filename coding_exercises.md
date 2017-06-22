## Coding Exercises
<!--- based on http://www.cs.cornell.edu/courses/cs1112/2017sp/#templates/exercises -->

### Part I: User input and looping
#### Hello
Create a file `Hello.java` such that running `javac Hello.java && java Hello` prints
```Hello world!```.
#### Hello by name
Modify `Hello.java` to prompt the user for their name, and greets them as follows:
```
$ javac Hello.java && java Hello
What is your name? asdfasdf
Hello asdfasdf!
```
(Hint: check out [this StackOverflow question](https://stackoverflow.com/questions/5287538/how-can-i-get-the-user-input-in-java). You can use `System.out.print()` to print text that does not end in a new line. )
#### Temperature conversion
Write a program `CtoF.java` that prompts a user for a temperature in Celsius and converts it to Fahrenheit.
(Recall that `degreeF = (9/5)*degreeC + 32`.)
For example, if the user enters 30, the output should look like:
```
$ javac CtoF.java && java CtoF
Enter a temperature in Celsius: 30
That's 86.0 degrees Fahrenheit!
```
Warning: Unintended [integer division](https://stackoverflow.com/questions/2909451/simple-division-in-java-is-this-a-bug-or-a-feature) may cause your program to print the wrong output!
#### Temperature conversion -- forever!
Add a while loop to `CtoF.java` to continue prompting the user forever.
(Now the user must type Control+C to quit the program!)
```
$ javac CtoF.java && java CtoF
Enter a temperature in Celsius: 0
That's 32.0 degrees Fahrenheit!
Enter a temperature in Celsius: 10
That's 50.0 degrees Fahrenheit!
Enter a temperature in Celsius: 20
That's 68.0 degrees Fahrenheit!
Enter a temperature in Celsius: ^C
```

#### Snake
Write a program `Snake.java` that asks a user for a number `n`, then prints a snake with `n` segments:
```
$ javac Snake.java&& java Snake
How many segments would you like your snake? 5
>(:)<><><><><>~
$java HeyYou
How many segments would you like your snake? 25
>(:)<><><><><><><><><><><><><><><><><><><><><><><><><>~
```
Hint: Use a `for` loop!

#### Diamond (tricky)
Write a program `Diamond.java` that prompts the user for a side length.
It then prints spaces and `*` characters to create a diamond that size:
```
$ javac Diamond.java && java Diamond
Diamond side length: 5
     *
    * *
   *   *
  *     *
 *       *
  *     *
   *   *
    * *
     *
$ javac Diamond.java&& java Diamond
Diamond side length: 10
          *
         * *
        *   *
       *     *
      *       *
     *         *
    *           *
   *             *
  *               *
 *                 *
  *               *
   *             *
    *           *
     *         *
      *       *
       *     *
        *   *
         * *
          *
```
Hint: First, concentrate on drawing the top half of the diamond.
You will need a `for` loop inside another `for` loop.
Inside the innermost `for` loop will be an `if` statement to determine whether the program should print a `*` or a space.
Good luck!

<!---
#### Random numbers and geometry
Consder a circle of radius r=1 centered at (0,0),
and a square with side length 2 centered at (0,0).
<img src="https://learntofish.files.wordpress.com/2010/10/circle_and_square.png" alt="Drawing" width=200/>

Compute a point with random coordinates (x,y) in the square by
```java
double x = 2.0 * java.util.Random() - 1.0;
double y = 2.0 * java.util.Random() - 1.0;
```
Print the random coordinates.
Print "INSIDE" if the point (x,y) is inside the circle, and "OUTSIDE" otherwise.
(Recall that the inside of the circle is the set of points (a,b) such that `a^2 + b^2 <= 1`.)

### Part III: TODO
-->



