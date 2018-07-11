# Recognize-named-entities-on-Twitter-with-LSTMs
We will use a recurrent neural network to solve Named Entity Recognition (NER) problem. NER is a common task in natural language processing systems. It serves for extraction such entities from the text as persons, organizations, locations, etc. In this task you will experiment to recognize named entities from Twitter.

For example, we want to extract persons' and organizations' names from the text.Than for the input text:
         
         __Ian Goodfellow works for Google Brain__

a NER model needs to provide the following sequence of tags:
       
         __B-PER I-PER    O     O   B-ORG  I-ORG__
Where *B-* and *I-* prefixes stand for the beginning and inside of the entity, while *O* stands for out of tag or no tag. Markup     with the prefix scheme is called *BIO markup*. This markup is introduced for distinguishing of consequent entities with similar types.

A solution of the task will be based on neural networks, particularly, on Bi-Directional Long Short-Term Memory Networks (Bi-LSTMs).

# Requirements

This tutorial requires the following packages:

* Python version 3.6
* Python 3.4 should be fine as well
likely Python 2.7 would be also fine, but who knows? :P
* numpy version 1.10 or later: http://www.numpy.org/
* tensorflow version 1.2 or later: https://www.tensorflow.org
* ipython/jupyter version 4.0 or later, with notebook support

(Optional but recommended):
* NVIDIA cuDNN if you have NVIDIA GPUs on your machines. https://developer.nvidia.com/rdp/cudnn-download
  The easiest way to get (most) these is to use an all-in-one installer such as Anaconda from Continuum. These are available for       multiple architectures.
