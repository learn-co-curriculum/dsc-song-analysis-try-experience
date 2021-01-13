# Song analysis with Python

## Objectives for this module
***  

* Understand variables and how they can be used
* Understand some different data types in Python including:
	* strings `str`
	* lists `list`
	* sets `set`
* Learn about some built in functions and methods in Python
* Discover some interesting ways to visualize data
* Observe the effects of parameters in a visualization

## What makes a hit song?

***

Think about your favorite song, and what you love about it. Maybe it's the singer or the guitar solo or the beat. You probably didn't think "I love how much it repeats itself!" What if I told you that repetitiveness is one of the key attributes of successful songs, and that there is data to back this up? In <a href="https://pudding.cool/2017/05/song-repetition/" target="_blank">this article</a>, Colin Morris asked and answered questions like this and came up with the conclusion that repetitiveness appears to be a driving force behind the 

In this module, we'll introduce you to a few of the fundamental components of Python and some ways you can apply this knowledge to data like these song lyrics. We'll explore some of the ways to organize data and some different visualizations you can use to gain insight into the song lyric data.


Here is a chart that Colin Morris produced showing some of the most repetitive popular artists.  
* How was something like this made and calculated?  
* What does this chart tell us?
In this module, we will take a look at some of the techniques used to gather data, organize it, and perform an analysis like this one.

![](https://learn-verified.s3.amazonaws.com/data-science-assets/song-chart.png)

This chart may be a bit confusing to read, let's take a look at a couple things before we move on. First, this is just a photo of an interactive version of the chart which you can see at the link at the beginning of the lesson.  There is much more information on the chart than we can see here, but this gives us some of the foundational information.
* The position on the x axis (left to right) tells us how repetitive the song is in percentage.  The further the song is to the right, the more repetitive the song is.  
* The label at the bottom is from the analysis.  In the analysis it was determined that the more repetitive the song is, the easier it is to digitally compress, so the reduction and repetitiveness of a song are the same.

## Recap

***

After finishing this module, you will have the foundation to start doing the kind of data analysis and visualization you see in Colin Morris' article. Awesome, right?