# Lists

## Objectives for this lesson

***

* Learn about the `list` data type
* Learn the syntax for strings `str` and numbers `int` in a `list`
* Create a list from a string of words using the `.split()` method
* Check the length of a list using the `len()` function

## The `list` data type

***

As you begin to take a look at this process, the first thing you'll notice is that our data is in the form of a simple string, all of the words are collected in one long string. In order to count the number of words, you first need to separate the string into individual words. One type of data structure you can use for this in Python is a list, which is indicated in Python with `list`.  

First, take a moment to familiarize yourself with the `list` data type and how to create a `list`.  You can create a `list` in Python by using square braces `[ ]` and separate each individual item in the list by a comma `,`.  

For example, if you want to create a list of the numbers 1 through 5, you can do it with the following code:  
`[1, 2, 3, 4, 5]`   
If you want to save this list for later use you need to assign it to a variable. For example, if you want to assign your list to the variable `numbers`, you can use the following code:  
`numbers = [1, 2, 3, 4, 5]`   

## Try it out

***

This list has been created for you in the code console below so you can see the result of this code.  Run the cell by clicking on the green arrow, then use the `print()` function to print the variable `numbers` to see the output. Your code should look like this:  
`print(numbers)`

<p><iframe src="https://repl.it/@DSExperience/ListofNumbers?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

Similarly, you can create a **list** of **strings**. For example, if you want to make a list called `pets` containing the types of pets in your household, such as a dog, cat, and bird, you can use the following code:  
```pets = ['dog', 'cat', 'bird']```  
Remember, to identify text as a string, you have to wrap it in quotes, either single quotes `' '` or double quotes `" "`, in Python the two are interchangeable.

## Try it out

***

Click on the green arrow in the code cell below, then use the `print()` function to print the variable `pets` to see the output. Your code should look like this:  
`print(pets)`  
>**Level Up** - In the code cell below, practice making your own list.  Try using more than one data type and see how it works.  

<p><iframe src="https://repl.it/@DSExperience/ListofStrings?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

## Apply it to our problem

***

Great, now that you understand **lists**, you can convert your continuous string of lyrics to a list of individual words using another built-in Python method `.split()`. The `.split()` method splits strings into individual elements based on the criteria you provide and puts those elements into a list. 

To use this method, you apply it to the end of the variable you want to split, and provide the separator as an argument to the method. The default behavior is to split on any whitespace, but you can specify the separator you would like to separate by.  For example, here are the directions in code:

```list_of_lyrics = lyrics.split(' ')```
 
for

> "split the string into a different entity every time you see a space"


## Try it out
***
In the code console below, we're creating `list_of_lyrics`. Let's see what this looks like. Run the console by clicking on the green arrow.  Now let's look at what `lyrics` looks like before we use this method, type `lyrics` in the console below to view it.  Then type in the variable name `list_of_lyrics` to see the output from the `.split()` method.

<p><iframe src="https://repl.it/@DSExperience/LyricSplit?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>

## The `len()` function

***

Ok, so this is a `list`, and as you can see, each word is now being treated as an individual **item**. Each individual item in a list is called an **element**. To see how many elements are in `list_of_lyrics`, you can use the function `len()`.  To use this function we must pass an iterable as an argument to the function, this is done by including the variable name in the parentheses like this: `len(list_of_lyrics)`  

## Try it out

***

In the code console below, you can check the length of `list_of_lyrics` using the `len()` function.  Try it out using the folowing code:  
```len(list_of_lyrics)```

<p><iframe src="https://repl.it/@DSExperience/LengthLyrics?lite=true" frameborder="0" width="100%" height="400px"></iframe></p>


## Recap

***

Great! You have learned how to split our string into a list of elements using the `.split()` method and to check the length of that list with the `len()` function.  You've also learned a few of the characteristics of lists and strings.  But remember the second step of **your plan** was to allocate space for each unique word. Now that you have a list of all words, you can isolate the individual words so you can keep track of how many times each one appears in our lyrics.  You can do this by creating a `set`. Let's look at sets in the next section.