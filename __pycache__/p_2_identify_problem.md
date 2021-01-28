# Analyzing One Song

## Objectives for this lesson

***

* Identify the problem we wish to address
* Develop a plan of attack to work through the problem 

## Identifying the problem

***

Let's take the song *Barbara Ann*, the most repetitive song of the Beach Boys which was remastered by the cast of *Saved by the Bell* in 1990.

![](https://learn-verified.s3.amazonaws.com/data-science-assets/saved-by-bell.gif)

How did the cast learn all of the words so easily?  Repetition. Here are some of the lyrics.


>Ah, ba ba ba ba Barbara Ann  
>Ba ba ba ba Barbara Ann 
>
>Oh Barbara Ann take my hand  
>Barbara Ann
>
>You got me rockin' and a-rollin'  
>Rockin' and a-reelin'  
>Barbara Ann ba ba Ba Barbara Ann  
>
>...more lyrics...  
>
>Ba ba ba ba Barbara Ann  
>Ba ba ba ba Barbara Ann


It keeps going, but you get the point.  

## Developing a plan of action

***

Now let's say that we wanted to count up how many times each word in the above selection appears.  Without a computer it would be difficult to organize and time consuming.  We would have to record all of the lyrics on paper, cross out all of the duplicates and then count the number of times each of the words occurs in the lyrics.  Also, we would not have the ability to do any visualizations.

With python, we will:
* Make a **list** of all of the words in the lyrics
* Make a **set** of all of the unique words
* Generate a word frequency table
* Chart the frequency table on a bar chart
* Create a WordCloud of the lyrics visualizing the higher frequency lyrics

Let's call these steps above **our plan**.  At the end of this lesson and after completing each step of our above plan, we will have a chart, like the one below, giving us a visualization of the most repetitious words in the Beach Boys' song, *Barbara Ann* as well as a WordCloud and some useful data structures for analysis.

<p style="text-align: center;">
	<img src='https://learn-co-curriculum.github.io/dsc-song-analysis-try-experience/Screen Shot 2021-01-12 at 4.00.18 PM.png' width='100%'></p>

## Recap

***

Great, now that we have a plan of action, let's translate our plan into code and make some visualizations.