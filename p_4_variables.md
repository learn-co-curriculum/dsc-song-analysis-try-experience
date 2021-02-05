# Variables

## Objectives for this lesson

***

* Create a variable
* Asign a value to a variable

## What is a variable?

***

Being able to input data is important, but you need to be able to store that data somehow.  To do this we will use a **variable**. Variables are used to store and access information, they also give us the ability to label our information with a descriptive name so our code can be understood better by others.  

Let's take a quick look at assigning a value to a variable. We use variables in coding so that we can write code that will not break when we change values so we do not have to re-write the code.  We assign a value to a variable by using the assignment operator `=`.  This assignment operator tells python to make our variable name represent the value we have given it.  

For example, if we wanted to assign the value `15` to the variable `number`, we would do that like this:  
`number = 15`  
Here we see that numeric values do not need quotes around them for Python to recognize them.  We can also assign a string value to a variable, like this:  
`word = 'Hello World'`  

## Try it out

***

Type these lines of code into the console below.  Once you have used our examples, try to change the values and see how it affects the output.  
`number = 15`  
`word = "Hello World!"`

Once you have assigned a value to your variable you can use the variable name in place of the data you assigned to it. Let's take a look at how we can do this.  
>In order to display the value assigned to a variable, you will need to pass the variable name to the `print()` function, like this:  
`print(number)` or `print(word)`

Try these examples out in the console below.

<iframe frameborder="0" width="100%" height="500px" src="https://repl.it/@DSExperience/Variables?lite=true"></iframe>

## Let's apply this to our problem

***

Now that you understand a little about how strings and variables work, let's assign our string of lyrics to a variable name. Let's call this variable `lyrics_sample`.  


```python
lyrics_sample = "Ah, Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann Oh Barbara Ann Take My Hand Barbara Ann You Got Me Rockin' And A-Rollin' Rockin' And A-Reelin' Barbara Ann Ba Ba Ba Barbara Ann ...More Lyrics... Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann"
```

Now whenever you type the word `lyrics_sample` into Python, you're referencing our string.

```python
"Ah, Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann Oh Barbara Ann Take My Hand Barbara Ann You Got Me Rockin' And A-Rollin' Rockin' And A-Reelin' Barbara Ann Ba Ba Ba Barbara Ann ...More Lyrics... Ba Ba Ba Ba Barbara Ann Ba Ba Ba Ba Barbara Ann"
```

## Try it out

***

You can try this yourself. We have created the variable `lyrics_sample` as shown above. If you click on the green arrow at the top of the interactive code console below, and type in the variable name `lyrics_sample` you'll see that Python will print out the lyrics for you!

<iframe frameborder="0" width="100%" height="500px" src="https://repl.it/@DSExperience/Load-the-data?lite=true=1"></iframe>

## Recap

***

Okay, great. You have now assigned the lyrics to our variable, `lyrics_sample` and you can use that to reference the string later in our code.  Now that you have learned about strings, let's learn how you can clean these strings up for our analysis. You will look at removing punctuation and normalizing the case of our text in the next lesson.