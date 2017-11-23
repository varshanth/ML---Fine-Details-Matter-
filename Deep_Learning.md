# Deep Learning
These resources are not mine and I do not claim that I have written/composed/presented them. They are an aggregation of publicly available resources. If any of the authors do not want their resources cited here, please report it as an issue and I will remove it from the repo at the earliest.

## Bible Videos of Deep Learning:
* CS231n Spring 2017 Stanford University  
https://www.youtube.com/playlist?list=PLC1qU-LWwrF64f4QKQT-Vg5Wr4qEE1Zxk
* Deep Learning.ai - Andrew NG  
https://www.youtube.com/channel/UCcIXc5mJsHVYTZR1maL5l9w

## Convolutional Neural Networks (CNN)
### Let's Diverge for a second: What is convolution? (and why should CNN be actually called Cross Correlation-al Neural Network)
This is optional, I spent some time on understanding the motivation behind a "convolutional" approach and these were the resources I referred. This isn't mathemetically important to CNN, but intuitively gives a good idea as to what the filters in the CNN are trying to achieve. 
* Obviously: https://en.wikipedia.org/wiki/Convolution
* Notice the animation: Remember the convolution operation is the integration, so it is the area UNDER the curve.  
http://mathworld.wolfram.com/Convolution.html
* Graphical Convolution Example: https://www.youtube.com/watch?v=zoRJZDiPGds
* Convolution vs Cross Correlation - Udacity : https://www.youtube.com/watch?v=C3EEy8adxvc

### Coming Back: CNN
* CS231n Lec 5 - Internals of CNN, receptive field, calculating new dimensions after convolution etc.
* Calculating the effective field of a CNN:  
http://shawnleezx.github.io/blog/2017/02/11/calculating-receptive-field-of-cnn/
* CS231n Lec 9 - CNN Architectures - VGGNet, GoogLeNet, ResNet, etc.

## Recurrent Neural Networks (RNN), Long Short Term Memory (LSTM) and Gated Recurrent Units (GRU)
* CS231n Lec 10 - RNN architecture, examples, drawbacks, requirement for LSTM, LSTM architecture etc.
* **Very important** to understand the difference between number of hidden units and RNN Cells because the definition in literature is different from that of implementation:   
https://stats.stackexchange.com/questions/241985/understanding-lstm-units-vs-cells  
In short, number of hidden units = size of the h vector, RNN cell in literature = A single RNN with a single hidden unit  
* How RNN & LSTMs work by Brandon Rohrer: https://www.youtube.com/watch?v=WCUNPb-5EYI
* Understanding LSTM Colah's blog - Simple explanation with motives:  
http://colah.github.io/posts/2015-08-Understanding-LSTMs/
* RNN & LSTMs from intuition to backpropagation with examples by Rohan and Lenny:  
https://ayearofai.com/rohan-lenny-3-recurrent-neural-networks-10300100899b
* GRU detailed: https://arxiv.org/pdf/1412.3555v1.pdf
* Relationship between LSTM, GRU & Highway Network:  
https://www.researchgate.net/profile/Tamer_Alkhouli/publication/307889449_LSTM_GRU_Highway_and_a_Bit_of_Attention_An_Empirical_Overview_for_Language_Modeling_in_Speech_Recognition/links/57d3433908ae6399a38da357/LSTM-GRU-Highway-and-a-Bit-of-Attention-An-Empirical-Overview-for-Language-Modeling-in-Speech-Recognition.pdf
* Brief summary of RNN, LSTM and GRU:  
https://www.slideshare.net/gakhov/recurrent-neural-networks-part-1-theory
* Using different batch sizes with LSTM:  
https://machinelearningmastery.com/use-different-batch-sizes-training-predicting-python-keras/
* Implementing mini batch algo in RNNs:  
https://www.quora.com/How-do-I-implement-mini-batch-algorithm-in-normal-RNN-and-Bidirectional-LSTM-RNN-for-NLP-task
* How are inputs fed to LSTM-RNN in mini batch method?  
https://www.quora.com/How-are-inputs-fed-into-the-LSTM-RNN-network-in-mini-batch-method


