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

## ***main.ipynb***
* The executable file


## ***The datasets Folder*** 
* <I>positive_samples.txt</I> (2000 Chinese positive reviews, label=1）
* <I>negative_samples.txt</I> (2000 Chinese negative reviews, label=0）

## ***The embeddings Folder***  
* <I>sgns.zhihu.bigram.bz2</I> （Pre-trained word vectors model）<br />Download from: https://github.com/Embedding/Chinese-Word-Vectors

