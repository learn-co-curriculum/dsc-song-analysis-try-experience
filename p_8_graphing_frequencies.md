# Graphing the Frequencies

## Objectives for this lesson

***

* Learn about the `dict` data type
* Create a frequency dictionary
* Learn about visualizations with `matplotlib`
* Create a bar chart

## The dictionary `dict` data type

***

Let's think about our lyrics. The information we are trying to organize is essentially a pair of `keys` (the lyric) and `values` (the number of occurrences of that lyric).  Python has a great data type that is perfect for this type of information, it is called a dictionary `dict`. A dictionary is a comma separated list of key and value pairs and in Python is denoted by the curly braces`{}` and each key value pair is joined with a colon `key:value`. The `value` is the important data you want to access or use, and the `key` is the address of that value.  We will not get into to much detail about dictionaries, for now we just need to know that it is a list of `key:value` pairs (where "keys" and "values" are separated by ":").  You could use a dictionary to store data about the artist of the song represented by key value pairs like this:  
`artist = {"name": "The Beatles", "genre": "Rock", "number of albums":12}`  

## Try it out

***

In the code console below, you can see a few examples of how to access the data in a dictionary. Run the code by clicking the green arrow and see the output from the code.

<iframe frameborder="0" width="100%" height="600px" src="https://repl.it/@DSExperience/Dictionary?lite=true"></iframe>


## Frequency

***

Now that you have a unique set of the words in the lyrics, you can begin to count how many times each word appears in the entire lyrics, this is often referred to as frequency.  To do this, you will once again use a for loop.  In the loop, you'll be iterating through the `set` `unique_words` and for each word you'll count the number of occurrences in the lyrics.  The results of each iteration will then be recorded in a dictionary as key value pairs.  Run the code console below to see the result of this action.

<iframe frameborder="0" width="100%" height="600px" src="https://repl.it/@DSExperience/LyricsDictionary?lite=true"></iframe>

Now that you have in the desired format, you can begin taking a look at the result of some of our work and begin to draw information from the data. In the graph generated below, you can see the frequencies of the first 6 words in the song.

<iframe frameborder="0" width="100%" height="600px" src="https://repl.it/@DSExperience/SongVisualization?lite=true"></iframe>

## Recap

***

In this section, you learned how to visualize data with a bar chart using matplotlib.  You also learned how to create a dictionary of key value pairs and created a dictionary of frequencies.