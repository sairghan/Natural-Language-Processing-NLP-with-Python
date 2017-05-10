# Natural-Language-Processing-NLP-with-Python

A simple tutorial on working with Language Data in Python using the Natural Language Toolkit (NLTK).

Prerequisites

    For this tutorial, you should have Python installed, as well as a local programming environment set up on your computer. 
    
**Step 1 — Importing NLTK**

Before we begin working, you should make sure that the NLTK module is installed. On the command line, you can check for NLTK by running the following command:

    $ python -c "import nltk"
   
If NLTK is installed, this command will execute with no error. You can check the installed version by running the following command:

    $ python -c "import nltk; print(nltk.__version__)"
    
You should have version 3.2.1 installed. We'll use NLTK's Twitter package in this tutorial and it requires NLTK 3.2.1.

If NLTK is not installed, you will receive an error message:

    Output
     Traceback (most recent call last): File "<string>", line 1, in <module> ImportError: No module named 'nltk'
 
The error message indicates that NLTK is not installed. You should download the library using pip.

    $ pip install nltk
     
Next, you will download the data and NLTK tools we will be working with in this tutorial.

**Step 2 — Downloading NLTK's Data and Tagger**

In this tutorial, we will use a Twitter corpus that we can download through NLTK. Specifically, we will work with NLTK's twitter_samples corpus. Let's download the corpus through the command line, like so:

    $ python -m nltk.downloader twitter_samples
    
If the command ran successfully, you should receive the following output:

    Output
     [nltk_data] Downloading package twitter_samples to
     [nltk_data]     /Users/sammy/nltk_data...
     [nltk_data]   Unzipping corpora/twitter_samples.zip.
     
Next, download the part-of-speech (POS) tagger. POS tagging is the process of labelling a word in a text as corresponding to a particular POS tag: nouns, verbs, adjectives, adverbs, etc. In this tutorial, we will specifically use NLTK's averaged_perceptron_tagger. The average perceptron tagger uses the perceptron algorithm to predict which POS tag is most likely given the word. Let's download the tagger, like so:

    $ python -m nltk.downloader averaged_perceptron_tagger
    
If the command ran successfully, you should receive the following output:

    Output
     [nltk_data] Downloading package averaged_perceptron_tagger to
     [nltk_data]     /Users/sammy/nltk_data...
     [nltk_data]   Unzipping taggers/averaged_perceptron_tagger.zip.
     
References

    https://www.digitalocean.com/community/tutorials/how-to-work-with-language-data-in-python-3-using-the-natural-language-toolkit-nltk
