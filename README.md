## OpenAI API Demo Application
This is the basic skeleton of a Flask application that takes a couple of text values as input 
and returns an output value.

The file base.html contains the basic structure of the web page. This 
can include the header, css definitions, footer, etc. With base.html taking care of the basics
we can create multiple pages that 'extend' base.html and add different content. In our case we 
may need to create 5 different pages for the different demos. These demos have the 
following input and output (draft, to be discussed):

1. Demo 1: Text Classification

Input 1: [string] A prompt with instructions on what features to extract from the article (e.g. topic, 
summary, sentiment, etc.)

Input 2: [string] Article Text 

Output: [json] A JSON with all the features described in the prompt
Ideal format of the output: for each key in the JSON, print key and value

Example:

Input 1: Given the following article, output a JSON file containing the topic, summary, and sentiment.

Input 2: Capitalism is very good for the rich and very bad for the poor. Blah Blah


Output:
Topic: Economics
Summary: This article is about capitalism.. 
Sentiment: Neutral

2.
3.

