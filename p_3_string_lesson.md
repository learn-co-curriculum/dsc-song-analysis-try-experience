# The string data type `str`

## Objectives for this lesson

***

* Use the `str` data type
* Create a `str` in the interactive code console

## Creating a `str`

***

To solve this problem with code, we do something similar to the manual card method we discussed in the last lesson which is to organize our lyrics into a `list`.  We start with our words in a `str`. We will learn about the `str` data type below, but first, let's see how it looks:


```python
"Ah, Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann Oh Barbara Ann Take My Hand Barbara Ann You Got Me Rockin' And A-Rollin' Rockin' And A-Reelin' Barbara Ann Ba Ba Ba Barbara Ann ...More Lyrics... Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann"
```


"Ah, Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann Oh Barbara Ann Take My Hand Barbara Ann You Got Me Rockin' And A-Rollin' Rockin' And A-Reelin' Barbara Ann Ba Ba Ba Barbara Ann ...More Lyrics... Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann"

> **Note:** What you see above in the first gray box is Python code - that is the code you would write.  What comes below that box is the output generated after running the code. So the output of creating a string is jest that same string - not very interesting.

## The `str` data type
***

Information in Python can be in many formats or data types, the most basic of these data types is a character, which is simply a letter, number, or some other form of punctuation.  When we put these characters together, we form what is called a *string* which is represented in Python by `str`. 

To create a `str` in Python, we place quotes at the start and end of text. The single quotes `''` and double quotes `""` are used interchangeably in Python and if we don't encase the `str` in either single or double quotes, Python will not create a string and may give us an error.

## Interactive code console

***

Throughout this module you will encounter our interactive code console, which you will use to practice writing the code you will learn in the lessons. This code console allows you to write and run code so you can see the results for yourself. 

To use the console, you'll first need to **initialize the console by clicking the green arrow**, as indicated by the arrow in the illustration below. 

<p style='text-align:center;'>
<img src='https://learn-co-curriculum.github.io/dsc-song-analysis-try-experience/replit_sample.png' width='75%'></p>

Once you have initialized the code console, you will be able to see the output of the provided code as well as type any commands or code as instructed in the material. You can type your code at the prompt as shown in the illustration below.

<p style='text-align:center;'>
<img src='https://learn-co-curriculum.github.io/dsc-song-analysis-try-experience/replit_prompt.png' width='75%'></p>

## Try it out
***

Great, now let's try to input something as a `str` - we'll start with something simple:  
`'Hello World'` or `"Hello World"`  
In the console below we can print ‘Hello World’ using the `print()` function, which looks like this:  
```python
print('Hello World')
```

Type this command in the code console below, then try it without the quotes, like this:
  
```python
print(Hello World)
```  

and look at the error message you encounter.

<iframe frameborder="0" width="100%" height="500px" src="https://repl.it/@DSExperience/Strings?lite=true"></iframe>

So, to avoid errors, we need quotes around our text to make a string.  Great, we know how to input some data, now let's learn how we can store that data so we can access it when we want it.

## Recap

***

In this lesson we learned about strings.  We learned that a string is just a group of characters and how to create and how not to create one. We also got a chance to use the interactive code console and write some code for ourselves. Now we will take a look at variables and how they store the information for us.  



