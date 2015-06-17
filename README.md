# Badges and Schedules

## Objectives

1. Utilize iteration
2. Define methods that use iteration and control the return values of those methods
3. Define methods that call other methods

## Instructions

In this lab you'll be learning how to iterate through an array and output the results in different ways. Your code will go in the "conference_badges.rb" file and you can run the test suite using the `rspec` command.

You're hosting a conference and need to print badges for the speakers. Each badge should say: "Hello, my name is _____."

1. Write a `badge_maker` method that will create and return this message, given a person's name.
ex:

    ```bash
    badge_maker("Arel")
    => "Hello, my name is Arel."
    ```

2. The list of speakers for your conference has been finalized. Your conference speakers are: `Edsger, Ada, Charles, Alan, Grace, Linus and Matz.` How you scored these luminaries is beyond me, but way to go! Now you'll want to get their badges printed. 
    
  * Write a `batch_badge_creator` method that takes a list of names as an argument and return a list of badge messages. 

3. You just realized that you also need to give each speaker a room assignment. Write a method called `assign_rooms` that takes the list of speakers that will assign each speaker to a room. Make sure that each room only has one speaker.
  * You have rooms 1-7. 
  * return a list of room assignments in the form of: "Hello, _____! You'll be assigned to room _____!"
  *  *Hint*: Think about how you will assign a room number to each person. Array items are indexed, meaning that you can access each element by it's index number. When you are iterating through an array using the `each` method, you can keep track of the index number of the current iteration. Look up how to do so and you should find a very helpful Ruby iteration method. 
  * *Hint*: Remember that the return value of the `each` method is the original array that you are calling it on. How can you collect or store the room assignment strings you are creating as you iterate and return them at the end of your `assign_rooms` method?

4. Now you have to tell the printer what to print. Create a method called `printer` that will output first the results of the `badge_creator` method and then of the `assign_rooms` method to the screen. 
  * *Hint*: Remember that methods can call other methods. If the return value of `assign_rooms` is an array of room assignments, how can you print out each assignment?


