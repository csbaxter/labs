# Mario

## World 1-1

Toward the beginning of World 1-1 in Nintendo's Super Mario Brothers, Mario must hop over adjacent pyramids of blocks, a la the below.

![screenshot of Mario jumping over adjacent pyramids](pyramids.png)

Let's recreate those pyramids in C, albeit in text, using at symbols (`@`) for bricks, a la the below. Each @ is a bit taller than it is wide, so the pyramids themselves are also taller than they are wide.

```
   @  @
  @@  @@
 @@@  @@@
@@@@  @@@@
```

The program we'll write will be called `mario`. And let's allow the user to decide just how tall the pyramids should be by first prompting them for a positive integer between 1 and 14, inclusive.

Here's how the program might work if the user inputs `8` when prompted:

```
$ ./mario
Height: 8
       @  @
      @@  @@
     @@@  @@@
    @@@@  @@@@
   @@@@@  @@@@@
  @@@@@@  @@@@@@
 @@@@@@@  @@@@@@@
@@@@@@@@  @@@@@@@@
```

Here's how the program might work if the user inputs `4` when prompted:

```
$ ./mario
Height: 4
   @  @
  @@  @@
 @@@  @@@
@@@@  @@@@
```

Here's how the program might work if the user inputs `2` when prompted:

```
$ ./mario
Height: 2
 @  @
@@  @@
```

And here's how the program might work if the user inputs `1` when prompted:

```
$ ./mario
Height: 1
@  @
```

If the user doesn't, in fact, input a positive integer between 1 and 14, inclusive, when prompted, the program should re-prompt the user until they cooperate:

```
$ ./mario
Height: -1
Height: 0
Height: 42
Height: 50
Height: 4
   @  @
  @@  @@
 @@@  @@@
@@@@  @@@@
```

Notice that width of the "gap" between adjacent pyramids is equal to two spaces.

Modify `mario.c` at right in such a way that it implements this program as described!

### How to Test Your Code

Does your code work as prescribed when you input

* `-1` (or other negative numbers)?
* `0`?
* `1` through `14`?
* `22` or other positive numbers?
* letters or words?
* no input at all, when you only hit Enter?

You can also execute the below to evaluate the correctness of your code using `check50`. But be sure to compile and test it yourself as well!

```
check50 csbaxter/problems/2021/x/mario/more
```

Execute the below to evaluate the style of your code using `style50`.

```
style50 mario.c
```

{% next %}

## How to Submit

Execute the below, logging in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.

```
submit50 csbaxter/problems/2021/x/mario/more
```
