# sentiment_analysis_imdb_reviews
Scripts to create a simple classifier to predict whether a review is a positive one or a negative one from raw text. BERT is also fine tuned to create a superior classifier.

This repo contains 2 scripts:
One creates classical ml models to classify whether a movie review is positive or negative. The other fine tunes BERT for the same task. You will need to complete the following steps to download and extract the data:

1) download the dataset from : http://ai.stanford.edu/~amaas/data/sentiment/
From the command line complete the following commands
2) `tar -xf aclImdb_v1.tar.gz`
3) `cd aclImdb && mkdir data`
4) ```for split in train test; do for sentiment in pos neg; do for file in $split/$sentiment/*; do cat $file >> data/full_${split}.txt; echo >> data/full_${split}.txt; done; done; done;```
