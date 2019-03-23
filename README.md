# TweetGenerator
Neural network model for writing tweets like @realDonaldTrump.
Inspired by: https://github.com/granilace/TweetGenerator

## Model
This model consists of two networks:
1. [Pre-trained RNN](http://nlp.fast.ai/category/classification.html) on Wikitext-103 and [fine tunned](https://nips2018creativity.github.io/doc/Transfer%20Learning%20for%20Style-Specific%20Text%20Generation.pdf) on last 2.7k tweets from Trump's Twitter loaded via Twitter API
2. 2-layer GRU char-RNN for proper letter capitalization

It also contains a prettifier module (beore capitalization) to clean sentences.


## Examples
* The Fake News is on frame. No official News was leaked.
* There is no reason to spend a year without a wall. We have the right to send leakers to the wall?
* The United States is with great progress with corrupt China, but I'm looking forward to doing very well! 

## Requirements
* fastai>=1.0
* PyTorch>=1.0
* numpy
* pandas
* python-twitter

## Authors
- @marianarfr
- @ricalanis
