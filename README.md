## ***Getting Started***

You need to use Google Colab platform. After opening the ***main.ipynb*** file in the link below, please complete Step 1 - 4 at the top. (Please do not run the code directly, otherwise compatibility errors will be reported)  
https://drive.google.com/drive/folders/185p_lZkp9sMGiSsS83KHBjRamtoFxjrv?usp=sharing

## ***Flowchart***
<center><img width=500 src="https://i.imgur.com/Ln5oRY1.png"></center>

## ***jieba: Chinese Word Segmentation Module***
* Related link: https://github.com/fxsjy/jieba  
* Some examples(based on the accurate mode of jieba) are shown below:  
<center><img width=600 src="https://i.imgur.com/5zQtA6O.png"></center>

## ***main.ipynb***
* The executable file

## ***The datasets Folder*** 
* <I>positive_samples.txt</I> (2000 Chinese positive reviews, label=1）
* <I>negative_samples.txt</I> (2000 Chinese negative reviews, label=0）

## ***The embeddings Folder***  
* <I>sgns.zhihu.bigram.bz2</I> （Pre-trained word vectors model）<br />Download from: https://github.com/Embedding/Chinese-Word-Vectors

## ***Model Training Results***
<center><img width=500 src="https://i.imgur.com/egoXJgu.png"></center>  
<center><img width=500 src="https://i.imgur.com/3V8QQX5.png"></center> 

## ***Model Test Results***
* model.evaluate  
<center><img width=700 src="https://i.imgur.com/jGUuXjh.png"></center>  

* model.predict  
<center><img width=600 src="https://i.imgur.com/vmmvES8.png"></center>  

* confusion matrix  
<center><img width=500 src="https://i.imgur.com/HBkh0Xz.png"></center>  

* False Positive Samples
<center><img width=700 src="https://i.imgur.com/z6ZaNmQ.png"></center> 
<center><img width=700 src="https://i.imgur.com/0yLWAgQ.png"></center> 
<center><img width=700 src="https://i.imgur.com/OyxaNuh.png"></center> 

* False Negative Samples
<center><img width=700 src="https://i.imgur.com/4okmAZI.png"></center> 
<center><img width=700 src="https://i.imgur.com/OTVC5Qq.png"></center> 
<center><img width=700 src="https://i.imgur.com/gsi9ITp.png"></center> 






