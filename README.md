# Chinese-Text-Sentiment-Analysis

前面这里先介绍一下，bulabulabula............  
Chinese text sentiment analysis using deep learning models such as LSTM, BiLSTM and GRU.

## Getting Started

The code is written in python and runs on Google Colab. To use it you will need:
* python 3.8.8
* numpy 1.21.6 
* matplotlib 3.2.2
* jieba (Chinese word segmentation module) v0.42.1  
* gensim 3.6.0 
* tensorflow 2.8.2

Before running <I>main.ipynb</I> make sure you load the <I>embedding</I> and <I>datasets</I> folders.  
(Depending on which Ide/running platform you are using, you may need to change the relative location of the <I>datasets</I> and <I>embedding</I> folders in the <I>main.ipynb</I> file.)

## jieba Usage
* `pip install jieba`
* `import jieba` <br />Related links: https://github.com/fxsjy/jieba

## The <I>datasets</I> Folder 
* <I>positive_samples.txt</I> (2000 Chinese positive reviews, label=1）
* <I>negative_samples.txt</I> (2000 Chinese negative reviews, label=0）

## The <I>embedding</I> Folder  
* <I>sgns.zhihu.bigram.bz2</I> （Pre-trained word vectors model）<br />Download from: https://github.com/Embedding/Chinese-Word-Vectors

