# Lists
## Objectives for this lesson

***

* Learn about the `list` data type
* Learn the syntax for strings `str` and numbers `int` in a `list`
* Create a list from a string of words using the `.split()` method
* Check the length of a list using the `len()` function

## The `list` data type

***

As we begin to take a look at this process, the first thing we notice is that our data is in the form of a simple string, all of the words are collected in one long string. In order to count the number of words, we first need to separate our string into individual words. One type of data structure we can use for this in Python is a **list**.  

First, let's take a moment to familiarize ourselves with the **list** data type and how to create a **list**.  We create a list in Python by using square braces `[ ]` and separate each individual item in the list by a comma `,`.  
For example, if we wanted to create a list of the numbers 1 through 5, we would do it with the following code:  
`[1, 2, 3, 4, 5]`   
If we wanted to save this list for later use we would need to assign it to a variable. For example if we wanted to assign our list to the variable `numbers` we would use the following code:  
`numbers = [1, 2, 3, 4, 5]`   

## Try it out

***

This list has been created for you in the code console below for you to see for yourself the result of this code.  Run the cell by clicking on the green arrow, then use the `print()` function to print the variable `numbers` to see the output. Your code should look like this:  
`print(numbers)`

<p><iframe src="https://repl.it/@DSExperience/ListofNumbers?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

Similarly, we can create a **list** of **strings**. For example, if we wanted to make a list called `pets` containing the types of pets in our household, such as a dog, cat, and bird, we would do it with the following code:  
```pets = ['dog', 'cat', 'bird']```  
Remember, to identify text as a string, we must wrap it in quotes, either single quotes `' '` or double quotes `" "`, in Python the two are interchangeable.

## Try it out

***

Click on the green arrow in the code cell below then use the `print()` function to print the variable `pets` to see the output. Your code should look like this:  
`print(pets)`  
>**Level Up** - In the code cell below, practice making your own list.  Try using more than one data type and see how it works.  

<p><iframe src="https://repl.it/@DSExperience/ListofStrings?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

## Apply it to our problem

***

Great, now that we understand **lists**, we can convert our continuous string of lyrics to a list of individual words using another built-in Python method `.split()`. The `.split()` method splits a into individual elements based on the criteria you provide and puts those elements into a list. 

To use this method, you apply it to the end of the variable you want to split, and you provide the separator as an argument to the method.  For example if you wanted to split The default behavior is to split on any whitespace, but you can specify the separator you would like to separate by.  For example, 

Here is how we tell the computer to do this: split the string into a different entity every time you see a space.  Here are those directions in code.  
```list_of_lyrics = lyrics.split(' ')```

## Try it out
***
In the code console below, you can see that we're creating `list_of_lyrics`. Let's see what this looks like. Run the console by clicking on the green arrow.  Now let's look at what `lyrics` looks like before we use this method, type `lyrics` in the console below to view it.  Then type in the variable name `list_of_lyrics` to see the output from the `.split()` method.

<p><iframe src="https://repl.it/@DSExperience/LyricSplit?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

## The `len()` function

***

Ok, so this is a `list`, and as you can see we are now treating each word as an individual **item**. Each individual item in a list is called an **element**. To see how many elements are in `list_of_lyrics`, we can use the function `len()`.  To use this function we must pass an iterable as an argument to the function, this is done by including the variable name in the parentheses like this: `len(list_of_lyrics)`  

## Try it out

***

In the code console below, you can check the length of `list_of_lyrics` using the `len()` function.  Try it out using the folowing code:  
```len(list_of_lyrics)```

<p><iframe src="https://repl.it/@DSExperience/LengthLyrics?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>


## Recap

***

Ok, great.  Now we have learned how to split our string into a list of elements using the `.split()` method and to check the length of that list with the `len()` function.  We have also learned a few of the characteristics of lists and strings.  But remember the second step of **our plan** was to allocate space for each unique word. Now that we have a list of all words, we can isolate the individual words so we can keep track of how many times each one appears in our lyrics.  We can do this by creating a `set`.  We will look at sets in the next section.