# Lesson \#1 - Introduction to Programming

This is it! This is why we're here - to become developers! No coding experience is required for this course, but if you happen to have some, feel free to skip this chapter and go straight into JavaScript. This section is going to introduce you to the fundamental building blocks of programming:

- Variables
- Operators
- Loops
- Conditionals
- Input
- Output.

Before we dive in let's make sure we are aligned on **what we mean by programming**:

- Programming is **storing and manipulating data** in an organized way **to accomplish a task**.

That's it. That's all it is. Some days it's going to feel overwhelming, and that's okay. The truth is that practically all programming problems can be traced back to these fundamentals, even if you find yourself working with frameworks and tools that abstract away the role of these core building blocks.

In your learning, if get lost or feel overwhelmed by a seemingly impossible problem, I encourage you to venture back here and revisit these fundamentals. Always remember that your problem can be solved with some configuration of these core building blocks. 

## Variables

Remember programming is **storing** and manipulating data in an organized manner to accomplish a task.

Variables are how we store data. It can be helpful to think of variables as named boxes where data is stored. In reality, data is stored in memory and variables are just a way to name a location in memory so we can easily find the data we stored there later. 

In JavaScript there are 6 primitive types of variables: 

1. boolean
2. string
3. number
4. null
5. undefined
6. symbol

For now, we're not going to concern ourselves with `null`, `undefined`, and `symbol`. These are special types whose use will become evident over time.

Let's dive into the `boolean`, `string`, and `number` and see what they are, exactly.

### Boolean

A `boolean` type variable can store one of two values: `true` or `false`. If you are a running a phone company and need to track whether or not a customer is eligible for an upgrade you would store this as a boolean. 

```js
isEligible = true;
```

### String

A `String` is a collection of characters like `"Hello future JavaScript rockstar"`. This is the data type that we'll use to store any and all text.

### Numbers

Unlike some other programming languages, JavaScript only has one number variable type. This means that the numbers can be whole or decimal values.

```js
a = 3

b = -2.53415
```

### Objects and Arrays

Two extremely important non-primitive data types are arrays and objects. 

Arrays are just lists of things `[1,2,5,7,8,9]` or `["Troy", "Abed", "Britta", "Shirley", "Jeff", "Pierce"]`. 

Objects are... a bit trickier. We'll do a quick overview of what they are and how they work, but keep in mind that this will all make more sense as you progress in your learning.

First, an object is a way of storing a state and behaviors. It is made up of many variables that together describe the complete object.

If you need to create several similar objects that are each unique in the content of their variables, you can use a class.

A class is like a blueprint for objects. 

For example, a class for a user of a service website might communicate something like "any objects created from this blueprint should have a String type variable called `name`, a number type variable called `age`, a boolean variable called `isEnrolled`, and a procedure for incrementing the age. 

So if my dog signed up for this website, his object would store that his `name` is Memphis, his `age` is 13, and `isEnrolled` is true. It would also store the increment age behavior so that on his birthday, we could execute that procedure and change his age to 14. 

This probably feels super abstract right now, but that's okay! It's supposed to. This is just preparing your mind for all the hands-on learning that's going to take place!

## Operators

Remember programming is storing and **manipulating** data in an organized manner to accomplish a task.

Operators allow you to perform arithmetic on values:

- `+` for addition

- `-` for subtraction

- `*` for multiplication

- `/` for division

- `%` to get the remainder of a division. 

Keep in mind that not all operators are used for arithmetic. Some are used for comparisons. 

- `>` returns true if the value preceding it is greater than the value that follows it. 

- `==` returns true if both values are equal. 

There are a few more operators than this, but the big takeaway is that operators are used to compare, combine, and alter values.  

Let's put this all together and get a peek at what this might look like in code. Perhaps our client is a car rental company and they need their application to verify that all renters are over 25: 

```js
age = 20;
threshold = 25;
isEligible = (age > threshold);
```

**Question:** What do you think `isEligible` will equal? 

**Answer:** False. `age` (20) is not greater than `threshold`, so th statement `age > threshold` evaluates to false.

## Conditionals

Remember programming is storing and manipulating data in an **organized** manner to accomplish a task.

Conditionals are used to control the flow of a program. They're sort of like switches. 

For example, a conditional can be used to cause one set of instructions to execute if a condition is true, and an entirely different set of instructions to execute if that condition is false. 

Think of it like this. Imagine that you come to a fork in the road on your way home from work. What you do next depends on the condition. **If** you are hungry, you go right towards the tofu-shack, **else** you go left towards home. 

For a more programming specific example, you could build a system for a wine distributor that allows a user to log in:

- `IF` they provided proper credentials. 

- `ELSE ` it will return an error message. 

You can even combine conditions in complex ways within your conditional. For example, using the same wine distributor application, you could permit a user to log in:

- `IF` they provide proper credentials.

- `AND` they are 21 or older.

Or perhaps you could clear a user:

- `IF` the user provides proper credentials.

- `AND` they at least 21-

- `OR` if they provide admin login credentials. 

As you can imagine, conditionals can be used to build quite complex applications. 

## Loops

Loops are another important way that you can control the order of operation in your program. As the name implies, loops allow you to do the same action repeatedly (like you're stuck in a loop) until some condition is met. You could print a name five times by using a loop with the condition 'iteration number is less than 5'. Makes sense, right? 

I know what you're thinking: "You have a typo. You said to print it 5 times and then said the condition would print while iteration number is **less than** 5." That's not a typo, though. In programming, you always start counting from index 0. So the first iteration is 0, then 1, then 2, then 3, then 4. 

<p align="center">
  <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/indexes-graphic.png" width="400" title="Indexes Graphic">
</p>

Printing your name 5 times isn't very practical, but there is a use-case for loops that are very practical and it's one you'll likely use all the time - iterating over an array. 

Want to print an array of elements? You need a loop. Increment every element in an array? Loop. Sum all the numbers in an array? Loop. Create complex SOM algorithms to identify hidden clusters in data? You'll need some loops there too. 

## Input and Output 

Lastly, we have input and output. Without these, we have a program that does... well something. Whatever it is, we can't see it,  and we can't use it. Input and Output allow users and other applications to interact with your application. For example:

- Input can mean numeric input, String input, or even button clicks, or sound (in the case of an audio recording software).

- Output can mean printing results, sending data to another system, rendering a display, or sending sick tunes to your speakers.

---

## Pseudo-coding

Phew... that was a lot. But that's pretty much all there is to programming. Sure there's a few more data structures and some advanced concepts, but at its root programming is combining a very limited number of tools in unique ways to accomplish something extraordinary! 

So now let's put it all together. Pull out your pen and paper. Write down the following: 

**A. Variable**

1. boolean
2. String
3. int
4. array

**B. Tools**

1. conditionals
2. loops
3. input
4. output

**C. Operators**

1. `+`
2. `-`
3. `*`
4. `/`
5. `<`
6. `>`
7. `==`

Write down which of the above you would use and in what order to create an application that takes in 2 numbers and outputs their sum?

Think it over. 

First, you need to get one **input**. 

Then you need to store it as a **number**. Why a number? Because I said the application takes in a number, not text. 

Then you get another **input** and store it as a **number** too. 

Now we use the `+` operator to add the numbers and store the result as a **number**.

Finally, we output the **result**.

So the solution is:

1. input
2. number
3. input
4. number 
5. `+`
6. number
7. output

In code, ignoring input for simplicity's sake, this might look something like: 

```JavaScript
num1 = 4;
num2 = 6;
sum = num1 + num2;
console.log(sum);
```

Even though this syntax is likely completely foreign to you, you can probably read it without much effort. Isn't that cool? 

Okay, so we walked through one together. Let's try a few more. 

But first...

### A pep talk

Research has shown that academic tenacity is often a greater predictor of academic performance than either ability or prior performance. What is academic tenacity? The ability to relish the opportunity to learn when confronted with challenges and withstand adversity to persevere towards a goal.

You are here to radically alter the path of your life in three months. Will it be easy? Heck no. At times you'll be frustrated. You'll doubt your abilities. You'll face problems that seem unsolvable. But if you persevere, if you continue to fight towards that goal, you will have the most transformative educational experience of your life. If you never stop fighting, who knows where you may go in life.

So let's dig in! Some of these are pretty tricky, so don't worry, the learning is in the struggle. Push yourself. Try different approaches. The frustration is where the learning takes place. Together, we are going to change your life, starting right now.

---

## Assignment

Now, it's your turn to do it on your own!

**A. Variable**

1. boolean
2. String
3. int
4. array

**B. Tools**

1. conditionals
2. loops
3. Input
4. Output

**C. Operators**

1. `+`
2. `-`
3. `*`
4. `/`
5. `<`
6. `>`
7. `==`

Write down which of the above you would use and in what order to create the following: 

1. An application that takes in two numbers, subtracts them, and prints the difference (no peeking at the one above)

2. An application that takes in two numbers and divides the first by the second if the first is less than the second. Otherwise, it multiplies the two. Print the result.

3. An application that takes in 2 numbers and a character. The character will be `"+"`, `"-"`, `"*"`, or `"/"`. Using the tools above, create a calculator that prints out the sum, difference, product, or quotient of the numbers. 

4. An application that prints the sum of an array of numbers. 

5. A tic tac toe game in which the user clicks to add an O or X (depending on whose turn it is). After each turn, if there are three of a kind in a row, the winner (X or O) is printed and the game ends. 


Once you've finished all 5 of the above, [check your answers](./answer-key.md).

