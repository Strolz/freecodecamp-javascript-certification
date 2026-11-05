Library Manager 
---------------

In previous lessons, you learned how to work with higher order functions like map, filter and reduce.

In this workshop, you will build a library manager app that will give you an opportunity to practice working with different higher order functions.

Step 1
------------

To get started, create a variable called library and assign it an empty array.

Step 2
------------

Inside the library array, create an object with the following properties and values:

Property	Value
title	"Your Next Five Moves: Master the Art of Business Strategy"
author	"Patrick Bet-David and Greg Dinkin"
about	"A book on how to plan ahead"
pages	320

Step 3
------------

Create another object inside the library array with the following properties and values:

Property	Value
title	"Atomic Habits"
author	"James Clear"
about	"A practical book about discarding bad habits and building good ones"
pages	320

Step 4
------------

Now would be a good time to start working on displaying the book information in the console. Over the next few steps, you will learn how to work with the map() method to achieve this goal.

Begin by logging the message "Books in the Library:\n" to the console. The newline character is added here to create a line break between this message and the list of books.

Step 5
------------

Next, create a function called getBookInformation with one parameter. This parameter will represent the array of books when the function is called. You could name the parameter catalog.

Step 6
------------

Inside the getBookInformation function, use the map() method on the catalog parameter to return a new array of just book titles. Refer to the example if you need help.

Step 7
------------

Now it is time to see what the result will look like in the console.

Below your getBookInformation function, add a console.log() and pass in a getBookInformation() function call with library for the argument.

When done correctly, you should see an array of book titles in the console.

Step 8
------------

Update your use of the map() method to instead return an array of strings in this format: TITLE by AUTHOR.

You will need to use either template literals or string concatenation with the + operator to achieve this result.

Step 9
------------

While the array of results is working, the final desired result should be a string listing all of the books with a title and author.

This is where the join() method comes in. In earlier lessons, you learned that the join() method is used to return a new string of all of the array elements concatenated into a single string, with a specified separator between each element.

The separator in this case is the \n which represents the newline character.

Chain the join() method with a \n for the separator to the map(). Now you should see a string in the console instead of the array of results.

Step 10
------------

For the next part of the workshop, you will focus on displaying a list of book summaries to the console.

Begin by logging the message "\nList of book summaries:\n" to the console.

Step 11
------------

To get a list of book summaries, you can use the about property of each book.

Create a getBookSummaries function with a single parameter, accepting an array with book objects. 

The getBookSummaries function should return an array of strings representing the summary for each book.

Step 12
------------

Just like in a prior step, the desired result would look nicer as a string instead of an array

Chain the join() method to your existing map() method and pass in "\n" for the separator to the join().

Then, below your getBookSummaries function, add a console.log(). The console statement should call the getBookSummaries function with library for the argument.

Now, you should see a string for the result in the console.

Step 13
------------

For this next part of the workshop, you are going to learn how to display a list of books by author.

Begin by logging the message "\nList of books by Arvid Kahl:\n" to the console.

Step 14
------------

Create a getBooksByAuthor function with two parameters - an array with book objects and a string with the author.

The function must return an array that contains the books by a particular author.

Step 15
------------

Now, it is time to test out your function.

Add a console.log() below your getBooksByAuthor() function.

Inside the console.log(), call the getBooksByAuthor() function with library and "Arvid Kahl" for arguments.

Now, you should see all of the books for that particular author in the console.

Step 16
------------

It would be nice to test our your getBooksByAuthor function with another author.

Begin by logging the message "\nList of books by James Clear:\n" to the console.

Below that console.log(), add another console.log(). Inside that console.log(), call the getBooksByAuthor() function with library and "James Clear" for arguments.

Now, you should see all of the books for that particular author in the console.

Step 17
------------

For the last part of the workshop, you will learn how to get the total number of pages for all of the books in the library.

Start by logging to the message "\nTotal number of pages for all library books:\n" to the console.

Step 18
------------

For the last step of the workshop, you will review how to work with the reduce() method. This method is used to process an array and condense it into a single value.

In the following example, the reducer function takes acc (which starts at 0, as specified by the second argument to reduce) and adds each number to it. This will return a sum of 15.

Create a getTotalPages function with a single parameter, accepting an array with book objects. The function should return the total number of pages in the books from the array passed to the function.

Lastly, add a console.log(getTotalPages(library)) below your getTotalPages function to see the result.

With that, your library manager workshop is complete!
