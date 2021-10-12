---
layout: archive
title: "Feed"
permalink: /feed/
author_profile: true
redirect_from:
  - /feed
---

*Fascinating ideas that I read*

## 	10th Oct 2021, 03:30 AM
Read another Andrej Karpathy's blog - [Short Story on AI](http://karpathy.github.io/2021/03/27/forward-pass/) in the middle of the night and it was mindblowing! <br>*Will add my thoughts soon!*

---
## 	9th Oct 2021, 08:00 AM
### Intro
Andrej Karpathy apart from being the director of AI and Autopilot Vision at Tesla and standing as the singular [human benchmark for ImageNet dataset](http://karpathy.github.io/2014/09/02/what-i-learned-from-competing-against-a-convnet-on-imagenet/) (yeah he classified all the images into 1000 classes after training for months!). 
He is very famous for his [blogs](http://karpathy.github.io/), specifically: [A Recipe for Training Neural Networks](http://karpathy.github.io/2019/04/25/recipe/) (inspired by his famous "most common neural network mistakes" tweet) and [The Unreasonable Effectiveness of Recurrent Neural Networks](http://karpathy.github.io/2015/05/21/rnn-effectiveness/). For a long time I wanted to read these blogs in its entirety and wasn't able to do it. This morning while taking a walk in the garden I decide to read the former blog: A Recipe for Training Neural Networks, and it was amazing!
### Motivation
He mentions 2 main ideas that motivated him to write this blog - Neural net training is a leaky abstraction, Neural net training fails silently. He is who coined the term "Programming 2.0" which encompasses this field of "Data-Driven Programming" (as George Hotz called it) where the directions of the program and results switch as compared to traditional programming:

<p align="center">
  <img src="https://sahilkhose.github.io/files/data_driven_programming.png" alt="Traditional vs ML programming image" width="450"/>
</p>

Precisely because of this nature of obtaining a black box function (program) to solve the problem in Programming 2.0 setup, even though everything could be correct syntactically, there are a lot of major errors and bugs which creep in and your neural network will be misconfigured which might still continue to learn, but its performance on test set will be trash or if it performs well on the test set, it will have learnt a wrong task altogether eg: Learning a snow classifier instead of the much more complex husky vs wolf task (shoutout to [Ankita's talk](https://drive.google.com/drive/folders/1LeJ-VOzK08jvw6ILYycikIZNcGpssCQO?usp=sharing) 36:05 timestamp) or a ruler classifier instead of cancer cell classifer!

### The recipe (Summary)
1. Become one with the data
2. Set up the end-to-end training/evaluation skeleton + get dumb baselines
    - fix random seed
    - simplify
    - add significant digits to your eval
    - verify loss @ init
    - init well
    - human baseline
    - input-independent baseline
    - overfit one batch
    - verify decreasing training loss
    - visualize just before the net
    - visualize prediction dynamics
    - ***use backprop to chart dependencies***
    - generalize a special case
3. Overfit
    - picking the model
    - adam is safe
    - complexify only one at a time
    - do not trust LR decay defaults
4. Regularize
    - get more data
    - data augment
    - creative augmentation
    - pretrain
    - stick with supervised learning
    - smaller input dimensionality 
    - smaller model size
    - decrease the batch size
    - drop
    - weight decay
    - early stopping
    - try a larger model
5. Tune
    - random over grid search
    - hyper-parameter optimization
6. Squeeze out the juice
    - ensembles
    - leave it training


### Most fascinating take away
Under tip 2: ***use backprop to chart dependencies*** <br>
Your deep learning models can get complicated very quick, and if you are writing the code from scratch, chances are you will make some mistakes which will make the model behave weirdly (high train and test metrics but not doing well on other downstream tasks). <br>
A relatively common bug is to use **view instead of permute**, which mixes the information across the batch dimension. And this hinders the performance in normal applications but when you have autoregressive models (eg: language models using next word prediction) model will have access to the next word and will propagate that directly to the output to get 0 train and test loss. But will not have learnt any meaningful representations of the word emeddings. (Another way this bug can creep in is while transfering dataset from one format to another, eg: Matlab uses index 1 and python (real programming languages) index 0, if we don't explicitly take care of the shift in index while importing the data which was stored in matlab, same data leak will occur) <br>
The way he suggests to debug this is to set the loss as the sum of all outputs of example i, run the backward pass all the way to the input, and ensure that you get a non-zero gradient only on the i-th input!! This proves that the information flow through the entire network for all the examples in the batch have completely independent paths and do not merge at any point!

### End Notes
- All of his tips are extremely useful for daily practices while working on new projects.
- 'Overfit on one batch' has saved a lot of compute
- 'Become one with the data' helped me solve a bug in a network which made it underperform for more than a month straight.
- 'Fix random seed' has helped a lot to reproduce the results when the training is very unstable.

This blog along with his twitter threads on most common mistakes has really helped me a lot as a DL practitioner.
This blog really got me interested to read more of his content, will read others soon!