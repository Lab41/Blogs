# Anything2Vec Code
## Karl Ni

For the original blog post, please see the original [Medium Article](https://gab41.lab41.org/anything2vec-e99ec0dc186#.roxvxhikl)

This is MATLAB/Octave code that should build some intuition about embedding any vectors into semantic space. It assumes that you have word vectors hough if you wanted to, you could optimize the word vectors as well. 

## Getting Started

If you don't have MATLAB, you'll need to install that or Octave.

## Where to Look

Start with the `anything2vec.m` script. This is the "main" script. Make sure you have the following variables in memory:

- `context` - of type `struct` the context of your vectors. The *i*th element is a collection of words related to the context of element *i*.
- `wordvecs` - of type 2D matrix (#words by #wordims), some word vectors you might've pretrained. (You could randomly init and optimize these as well..)
- `wordcounts` - array of size #words, detailing how often the words occur.
