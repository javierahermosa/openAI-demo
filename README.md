# OpenAI API Demo Application
This is the basic skeleton of a Flask application that takes a couple of text values as input 
and returns an output value.

The file base.html contains the basic structure of the web page. This 
can include the header, css definitions, footer, etc. With base.html taking care of the basics
we can create multiple pages that 'extend' base.html and add different content. In our case we 
may need to create 5 different pages for the different demos. These demos have the 
following input and output (draft, to be discussed):

### Demo 1: Text Classifier

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

### Demo 2: Vision
In this demo we will use the API to describe an image, compare two images, or understand hand-written notes. 

Input 1: [string] A Text Prompt

Input 2: [TBD] An image

Input 3: [TBD] A second image

Output: [JSON] A JSON with 3-4 text fields (description, transcription, translation, explanation).


### Demo 3: Image editing
In this demo, we will edit images by creating a new image from an old image + a mask.

Input 1: [TBD] An image (or image path?).

Input 2: [TBD] A mask image (or mask path?).

Output: [TBD] An image. Ideally we should render the resulting image on the right page. The output of the model is either a web url or a b64_json.

### Demo 4: Vision using video and reproduction using audio
In this demo we will show how to describe a video, and the description will be in the form of text and an audio file that will be played to the audience.

Input: [TBD] A video (or video path?)

Output: [string] text describing the video and the possibility of reproducing the MP3 audio.

### Demo 5: Having a conversation with a document
In this demo we will test the concept of memory and retrieval, by chatting with a long document.

Input 1: A pdf file such an astronomy paper, or EV paper.
Input 2: [string] A prompt with some questions about the paper

Output 1: [string] A summary of the paper.
Output 2: [string] An answer to the question
... the conversation will continue until the user ends it.

### Demo 6: Fine tuning 
### Demo 7: Assistants (playground)
### Demo 8: GPTs (playground)

