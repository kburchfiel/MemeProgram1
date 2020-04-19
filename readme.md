This is a silly C++ program that provides you with a crude "animated desktop background" (really just a command prompt) in front of which you can place other windows on your computer. I do **not** recommend it for anyone who has epilepsy.
 
The second version of this program corrected a drawback noted by Chris Y on my corresponding Youtube video(https://www.youtube.com/watch?v=4sGGwS4ZI7o). Chris noted that the for loop (x = 1; x > 0; ++x that this program originally used would stop once the value of x overflowed into a negative number. Since I wish for this to be a program that continues indefinitely, I changed it to incorporate a while (true) loop that won't end until the user exits the program. 

There are lots of ways to change the "animation." For instance, try removing the space that proceeds x in std::cout. Alternatively, you can make x a double with the initial value 1.0001 and then have it multiply itself by 1.0001 within the while loop. 

When this program runs on my computer, it appears to display updated versions of x ( . . . 101, 102, 103 . . . ) nearly 5,000 times per second if I keep the command prompt very small. If this speed remains constant, it should take a little over 5 days for x to overflow and become negative (e.g. . . . 2,147,483,646, 2,147,483,647, -2,147,483,648, -2,147,483,647 . . . ). I wonder to what extent this timing would vary among different computers. 

I recognize the indentation of the code is not ideal, but I wanted to say that the program used only 4 lines of code. Using the auto-indentation feature in Visual Studio Code brings the program up to 10 lines of code.

--Kenneth Burchfiel, 2020-04-18
