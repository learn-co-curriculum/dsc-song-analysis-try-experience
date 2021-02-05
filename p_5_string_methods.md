# String Methods

## Objectives for this lesson

***

* Methods of the `str` function
* Find documentation on Python packages
* Clean the data with the `.replace()` method
* Use a method with an argument
* Change case of a string with the `.lower()` method


## Cleaning the data

***

In order to process the data effectively, you need to make sure that it is clean. In this particular case, this means that you will need to remove extraneous punctuation and normalize the case of the text. This can be accomplished by using built-in methods in Python's string module. Python has many useful methods for strings, but we will just introduce you to a couple in this lesson. 

>When you encounter a new collection of python commands, sometimes referred to as packages or libraries, it is helpful to read through the documentation and familiarize yourself with the commands that are avaliable and the types of arguments they take by visiting the documentation page. Take a moment to look at some of the methods that python has built-into the `str()` function <a href="https://docs.python.org/2/library/stdtypes.html#string-methods" target="blank">here</a>. You can see a sample of the documentation below.

<div class="fs-browser-header">
	<div class="fs-browser-dots"></div>
	<strong>https://docs.python.org/2/library/stdtypes.html#string-methods</strong>
</div>
<div class="fs-browser">
<img src="https://learn-co-curriculum.github.io/dsc-song-analysis-try-experience/string_function_docs.png"></img>
</div>

## The `.lower()` method

***

Python is sensitive in how it looks at data, for instance, `'Ba'` and `'ba'` will be viewed as two completly different words. This is due to the fact that each form of a letter is it's own character, so `'B'` is different from `'b'`. We will address this with the `.lower()` method. The `.lower()` method is an attribute of the string function and changes the case of all characters to lower case. For example:
`'Barbara Ann'` then becomes `'barbara ann'`.  

## Try it out

***

The code console below will demonstrate how the `.lower()` method works.  We have saved a string with the variable name `data`. In the first line of the output, you see the result of `print(data)`. In the second part of the output, you see the result of applying the `.lower()` method to `data` which looks like this: `print(data.lower())`.
Run the console by clicking on the green arrow to view the output of the code.

>**Level Up** - use the code console to create your own variable and assign your name to it with the proper capitalization, then use the `.lower()` method to change your name to lower case.

<iframe frameborder="0" width="100%" height="600px" src="https://repl.it/@DSExperience/Lower-Case-Method?lite=true"></iframe>

## The `.replace()` method

***

When analyzing text, you need to make sure that the data is free of all unnecessary punctuation as these characters can throw off the analysis and cause some undesired results.  Below, you'll use the `.replace()` method to address some of these items such as punctuation and extra words. 

Some methods require input in order to work properly.  In our case, the `.replace()` method takes in two arguments separated by a comma: the first argument is the substring you want to remove and the second is the substring you wish to replace it with.  For example, if you wanted to replace a `?` with a `!` the code would look like this:  
`new_string = old_string.replace('?', '!')`  
> Notice that you have to assign the result to a variable, this is necessary since this method is considered "non-destructive". This means the method does not change the original string.  
Lets look at an example of the `.replace()` method to see how this works in the code console below.

## Try it out

***

In the code below, we are removing the punctuation from the sentence using the `.replace()` method.  You will first see how the apostrophe is removed and replaced with nothing.  The apostrophe is a `str`, so you need to wrap it in quotes, like this: `"'"`. This is the perfect example that demonstrates the need for the two different types of quotes.  We use the double quotes here because the single quotes will get confusing for Python and we will encounter a syntax error. We are replacing the apostrophe `"'"` with a `str` of nothing `''`.  Run the code console below, then type in the following code to see how this works.  
`lyrics.replace("'", '')`

<iframe frameborder="0" width="100%" height="500px" src="https://repl.it/@DSExperience/LowerCase?lite=true"></iframe>

## Let's apply this to our problem

***

Below is the sample of the lyrics you have been working with.  Up to this point, you have just been working with a little piece of the song to make things easy, from this point forward, you will be working with the full set of lyrics from the song *Barbara Ann*.  In the sample below, you can see that there are many different characters that are not needed for our analysis, they have been highlighted to make it easier for you to see them.

"Ah`,` Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann Oh Barbara Ann Take My Hand Barbara Ann You Got Me Rockin`'` And A`-`Rollin`'` Rockin`'` And A`-`Reelin`'` Barbara Ann Ba Ba Ba Barbara Ann, Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann"

To begin cleaning our data, you will first apply the `.lower()` method to normalize the case of the text.

## Try it out

***

Run the code console below to see the output from the `.lower()` method. 

<iframe frameborder="0" width="100%" height="900px" src="https://repl.it/@DSExperience/Lowerlyrics?lite=true"></iframe>

Great, now you have the text case normalized, you can remove the unnecessary punctuation. 

## Try it out

***

To see how the `.replace()` method replaces these items in our data, you can run the code console below, simply click on the green arrow to see the data before and after. You can also print out `lyrics_before` and `lyrics_after` and look at each one individually.

<iframe frameborder="0" width="100%" height="900px" src="https://repl.it/@DSExperience/stringmethods?lite=true"></iframe>

The sample of the song lyrics is composed of just a few lyrics and each of those lyrics is capitalized. The whole song is a bit longer and has some words capitalized and some lower case. This can cause an issue for the analysis since python is case sensitive and will see the same word both capitalized and lower case as two different words.  For example 'Ba' and 'ba'. Python identifies each of these as a different word. This is an issue with the whole song lyrics, so we will use another string method `.lower()` to help with this. The `.lower()` method works on a string. Since `list_of_lyrics` is a collection of strings, you can use a `for loop` to iterate through the list and apply the method to each string. 

## Recap

***

In this lesson, you explored a couple of ways data can be cleaned for analysis. You looked at two string methods: `.replace()` and `.lower()` and how these methods can be used to clean the data and get it to a state that will lend itself to a more accurate analysis. If you remember **our plan**, the first step was to place each word on a separate index card, but strings are **not** good for separating our text into individual words.  For that, you need a new data structure called a **list**.  In the next lesson, you will be introduced to the **list** `list` data type.
