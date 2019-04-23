# Lesson \#4 - Node (JavaScript) Application

Congratulations for having completed the lesson on JavaScript! Be sure to bookmark the [JavaScript Workbook](https://javascript-workbook.netlify.com/) so you can reference it during this lesson.

Now we'll be jumping into Node.js! Node.js allows us to use JavaScript outside of a browser. You can think of Node.js as a rough equivalent to most other programming languages such as Python or Ruby.

In this lesson, we'll be using only our terminal/GitBash to run our programs. Executing files through the Terimanl/GitBash is a skill that will come in handy as we work with Angular in the future. But for now, let's dive into how to do that using Node.js!

Start by creating a new folder called, "new-node". We'll be working out of this folder throughout this lesson so make sure that you navigate to it in your terminal/GitBash.

Within our "new-node" folder, create a new file called, "index.js". This is the file that we will be opening using our terminal/GitBash so be sure to remember the file name! And inside of "index.js", create a console log that will print "Hello World!".

Navigate back to your terminal/GitBash and while you are within the "new-node" folder, type "node index.js". 

```
node index.js
```

Voila! You've just written JavaScript and executed the program within your Terminal/GitBash!

Now you might be wondering what else you can do. For the most part, you can approach Node.js the same way you do JavaScript because Node.js *IS* JavaScript! Let's put that to the test by creating a new function that simply prints out "Hello World!". Don't forget to instantiate, or call, the function after creating it.

After having done that, run the program and make sure that it functions properly. If it functions properly move on to the assignment for this lesson! If you were unable to execute the program and have it print "Hello World!" in the terminal/GitBash, follow the troubleshooting steps below!

#### Did you get an error?

*Yes, it says: 'node' is not recognized as an internal or external command.*
Make sure that you have downloaded and installed the latest version of Node.js! Refer back to [Chapter 3, Lesson 3](sub-modules/chapter3/lesson3.md) if you need a refresher on how to do this.

*Yes, it says: Error: Cannot find module ...*
Check for any spelling errors when typing your Node command in the terminal/GitBash. You may have mispelled the file name.

*No, no errors*
Move on to the next troubleshooting step!

#### Did you get something to print out?

*No, it didn't print anything out*
Check your code to make sure that you don't have any typos and that you are actually calling the function.

*Yes but it printed something different.*
Then you're likely working out of a different folder! Navigate to the "new-node" folder that you've created during this lesson.

*Yes, it printed out "Hello World!".*
Fantastic! Now tackle the assignment!


---

### Assignment

For this activity we'll be tying together concepts learned from all of the previous chapters. You'll be creating a function that checks to see if a number that is passed in is greater than or less than 10. If a number is not passed into the function, print out "Hey! That's not a number!" 5 times. Make sure that you use a for loop for this. 

If a number is passed into the function and if that number is greater than 10, print out "Hey! That's a large number!". If that number is less than 10, print out "Hey! That's a small number!".

Start by creating a new GitHub repository called, "prework-node" and cloning it down. 

Use the following starter code and create a function called, "loopyThing", that will accomplish the task!

```js
// Your code here!

loopyThing(12)
console.log("===========================")
loopyThing(5)
```

After writing the code and testing to ensure that the program works, push your changes to the GitHub repo.

Take your time with this activity and look up any resources you might need to accomplish this task. Remember, you can always refer back to the [JavaScript Workbook](https://javascript-workbook.netlify.com/) as well.
