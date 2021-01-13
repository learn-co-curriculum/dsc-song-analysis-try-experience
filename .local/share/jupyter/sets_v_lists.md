# Sets vs Lists

## Objectives for this lesson
***
* Learn the `set` data type
* Create a `set` from a `list`
* Discover the difference between `set` and `list`
* Create a `set` from our lyrics

## The `set` data type
***
A `list` can contain as many duplicates of each item as necessary, but sometimes we want a list of which unique items are in our list. We are able to do this with the `set()` method.  The `set()` method creates a collection of all of the unique elements from the collection that is passed to it. Let's take a look at sets before we get back to our project.

A `set` is a collection of unique elements and is un-ordered and un-indexed. As an example the list `[1, 2, 2, 4, 4, 5, 6]` when converted to a `set` would result in the following set `{1, 2, 4, 5, 6}`.  

## Try it out
***
Run the code console below and see for yourself how this works.  Click on the green arrow to see the output from this code. 

<iframe frameborder="0" width="100%" height="400px" src="https://repl.it/@DSExperience/ListandSet?lite=true"></iframe>

## `set` order doesn't matter
***
One of the properties of a _set_ is that the order of the elements in the set doesn't matter. What does that mean? Let's look at a simple example. `set_1` and `set_2` below are two sets, each contains the same elements (1, 2 and 3), but as you can see, they are in different orders. 

## Try it out
***
You can see this property by running the code in the console below. Click the green arrow to see the output from this code.

<iframe frameborder="0" width="100%" height="400px" src="https://repl.it/@DSExperience/SetCompare?lite=true"></iframe>

## What about lists?
Python tells us that these sets are identical! With the `set` data type, the order is not important. Wow! What about lists, do they have these same properties as well? Let's see how a list acts in the same code.

## Try it out
***
Run the code console below to see if a `list` shares the same properties with a `set`.

<iframe frameborder="0" width="100%" height="400px" src="https://repl.it/@DSExperience/ListCompare?lite=true"></iframe>


## Let's apply it to our problem
***
We just learned that order matters for lists, but not sets! Why does this matter to us? One of the steps in **our plan** was:

> - Designate a spot for each unique word in our index cards

In our case a `set` will create a collection of all of the individual words in the song, but as we have seen, the order will not remain. We will first get the set of unique words and then we will convert it to a list so that we can maintain the order integrity. Our first step is to create the set of unique words and we can accomplish this with the following code:
`unique_words = set(list_of_lyrics)`

## Try it out
***
Click on the green arrow and type in `unique_words` to see what this set looks like.

<iframe frameborder="0" width="100%" height="300px" src="https://repl.it/@DSExperience/UniqueWords?lite=true"></iframe>

We can see here that our list of unique words is significantly smaller than our total list of words.  How much smaller? Let's run the codeblock below to find out.

<iframe frameborder="0" width="100%" height="700px" src="https://repl.it/@DSExperience/Setcompare?lite=true"></iframe>

That's a lot!

So, there's a lot of repetition in `Barbara Ann`.  It's time to keep track of each word and the number of occurrences of each word.


One of our goals is to present our list of repetitions almost as a table, with a (unique) word to the left and the number of occurrences to the right, this is known as a frequency table, but we will get deeper into that in a later lesson.  Below is an example of what a frequency table looks like:  

| unique_words        | count           |
| ------------- |:-------------:|
| Ann     | 2 |
| Barbara     | 3 |
| Ba     | 8 |

Now that we have a collection with the unique words, we need to make sure our order of unique words is fixed, because we will start matching a value to it (the value being equal to how often the word occurs in the song). So let's convert our `unique_words` `set` to a `list`. We can do this by using one simple line of code and the `list()` function.  We will simply provide our set as an argument to the `list()` function like this:  
`unique_words = list(unique_words)`

We can check that this worked by passing the variable name `unique_words` as an arguement to the `type()` function.  

## Try it out
***
Run the cell below to see how this works.

<iframe frameborder="0" width="100%" height="500px" src="https://repl.it/@DSExperience/TypeFunction?lite=true"></iframe>
	
## Recap
***

In this lesson we learned the difference between a `list` and a `set`.  We also discovered that the order is not important in a `set`, but that a `list` will maintain the order of the data.  We also looked a a function to check the type of data that is referenced by a variable as well as how to convert an unordered `set` back to an ordered `list`.  Now that we have the data in the format we need for our analysis, we can move on an begin to count the occurrences of each word in our lyrics. We will learn how we can create a collection of key, value pairs by using annother data type called a dictionary `dict` in the next section.



