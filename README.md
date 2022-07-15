# Chinese-Text-Sentiment-Analysis
Chinese text sentiment analysis using deep learning models such as LSTM, BiLSTM and GRU.

$$positive->label('美味')=1$$

$$negative->label('难吃')=0$$

## ***Flowchart***
<center><img width=500 src="https://i.imgur.com/Ln5oRY1.png"></center>

## ***Getting Started***

The code is written in python and runs on Google Colab (CPU, not GPU). To use it you will need:
* python 3.7.13
* numpy 1.19.5
* matplotlib 3.2.2
* jieba 0.42.1  
* gensim 4.1.2 
* tensorflow 2.5.0

Before running <I>main.ipynb</I> make sure you load the <I>embeddings</I> and <I>datasets</I> folders.  

## ***jieba Usage***
* `pip install jieba`
* `import jieba` <br />Related links: https://github.com/fxsjy/jieba
<center><img width=600 src="https://i.imgur.com/5zQtA6O.png"></center>

## ***main.ipynb***
* The executable file


## ***The datasets Folder*** 
* <I>positive_samples.txt</I> (2000 Chinese positive reviews, label=1）
* <I>negative_samples.txt</I> (2000 Chinese negative reviews, label=0）

## ***The embeddings Folder***  
* <I>sgns.zhihu.bigram.bz2</I> （Pre-trained word vectors model）<br />Download from: https://github.com/Embedding/Chinese-Word-Vectors

## ***Model Building***
We tried several neural network structures, and because the training samples were relatively small, the training process did not take long to complete.  
* GRU: The test samples could achieve 87% accuracy if GRU was used. However, when I tested my own text content, I found that the output of the last layer of the GRU activation function was all around 0.5, indicating that the model's judgement was not very clear, and after testing, I found that the model sometimes missed the judgement for negative sentences. We would expect the output to be close to 0 for negative samples and close to 1 for positive samples rather than hovering between 0.5.
* Single LSTM, stacked LSTM and BiLSTM: We tested both LSTM and BiLSTM and found that BiLSTM performed best, with LSTM performing slightly better than GRU, probably because BiLSTM has better memory for longer sentence structures.
* After Embedding the first layer we used BiLSTM to return sequences, then the second layer of 16 units of LSTM did not return sequences but only the final result, and finally a fully linked layer with a sigmoid activation function to output the result.

## ***Test Results***
* model.evaluate  
<center><img width=700 src="https://i.imgur.com/2K9V6zW.png"></center>  

* model.predict  
<center><img width=600 src="https://i.imgur.com/vmmvES8.png"></center>  

* confusion matrix  
<center><img width=500 src="https://i.imgur.com/h0JnFPr.png"></center>  

## ***Error Analysis***
Through our analysis, we find that the meaning of the misclassified text is mostly ambiguous, and even humans can not easily determine the polarity. For example, this sentence with index 305 seems to have no element of satisfaction at all, but this example rating is marked as positive in the training sample, and the prediction of a negative rating made by our model seems reasonable.
* False Positive Samples
<center><img width=700 src="https://i.imgur.com/z6ZaNmQ.png"></center> 
<center><img width=700 src="https://i.imgur.com/z6ZaNmQ.png"></center> 
<center><img width=700 src="https://i.imgur.com/z6ZaNmQ.png"></center> 

* False Negative Samples
<center><img width=700 src="https://i.imgur.com/8mT1TtM.png"></center> https://i.imgur.com/z6ZaNmQ.png
<center><img width=700 src="https://i.imgur.com/8mT1TtM.png"></center> https://i.imgur.com/z6ZaNmQ.png
<center><img width=700 src="https://i.imgur.com/8mT1TtM.png"></center> https://i.imgur.com/z6ZaNmQ.png






