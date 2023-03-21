# Dog-MGAN - Course Project
Dog Image Generation w/ MGANs

## Table of contents
* [General Info](#general-info)
* [Technologies](#technologies)
* [Process](#process)
* [Conclusions](#conclusions)

## General Info
This was a project for a masters course at CU in which we were to compete in the Kaggle [Generative Dog Images](https://www.kaggle.com/competitions/generative-dog-images) challenge.
This challenge wanted us to utilize GANs to create images of dogs which were then scored based on classifications from pre-trained neural networks.
The assignment required a single .ipynb file as the submission, so the whole project is contained within - including reasonings and justifications of methods used.

## Technologies
- numpy
- pandas
- tensorflow / keras
- glob
- seaborn
- matplotlib

## Process
Something of note for this challenge was that almost all of the top scoring notebooks used almost identical code.  Reading through submitted projects showed why this was - all of them used a method that seemed to have come from Chris Deotte's Dog Memorizer GAN [notebook](https://www.kaggle.com/code/cdeotte/dog-memorizer-gan/notebook).
He showed that using a Memorizer and Generalizing generator in tandem allows for easy memorization of all the images in the training set, while the generalizer attempts to 'generalize' the 
coached images into being more than just a re-print of that which was memorized.  Because I had previously worked with GANs but not with a memorizer/generalizer, along with the fact that the original notebook won a medal for this method, I chose to also use these generators and see what it was all about.

## Conclusions
What I did mirrored much of what was done in other notebooks for this competition, and to be honest there wasn't much to it.  The memorizer memorized the training data and then the generalizer made it look a little different, just as expected.  What was unexpected was that this was allowed as a submission to the competition since there is no real 'learning' going on with our model - we just choose how much of a distortion to add to the pixels of true images.  
I went in to more detail on the process of testing the generators and my findings in the notebook, but there isn't much more to say.
