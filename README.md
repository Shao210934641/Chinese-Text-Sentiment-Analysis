# Chinese-Text-Sentiment-Analysis

前面这里先介绍一下，bulabulabula............  
Chinese text sentiment analysis using deep learning models such as LSTM, BiLSTM and GRU.

## Getting Started

The code is written in python. To use it you will need:
* python 3.8.8
* numpy 1.21.6 
* matplotlib 3.2.2 
* jieba (Chinese word segmentation module) v0.42.1 
* tensorflow 2.8.2

Before running main.ipynb make sure you load the 'embedding' and 'datasets' folders.

## jieba Usage
* pip install jieba 
* import jieba 

## the datasets Folder 
* positive_samples.txt (2000 positive reviews, label=1）
* negative_samples.txt (2000 negative reviews, label=0）

## the embedding Folder  
* sgns.zhihu.bigram.bz2 （Pre-trained word vectors model）<br />Download from: https://github.com/Embedding/Chinese-Word-Vectors

