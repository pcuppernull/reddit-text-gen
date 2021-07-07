# reddit-text-gen

This repository reproduces the results of my final project for the course Thinking With Deep Learning (Spring 2021) at the University of Chicago, taught by Dr. James Evans. In this project, I use data from Reddit to fine tune a series of GPT-2 text generation models. I use monthly snapshots of data from r/Conservative, r/Liberal, and r/Socialism from 2017-2019 to train 52 unique text generation models, to which I pose various prompts that generate text regarding the societal impact of social media. This serves as a "survey" of Reddit users, and I exploit variation in the results over time to assess how the perception of the impact of social media on society has evolved between people of different political ideologies. 

At a high level, I find that liberals more so than conservatives have grown to view social media -- specifically Facebook -- as more impactful on society in recent years. These views developed most significantly following the public revelations of Facebook's Cambridge Analytica scandal in 2018.

There are five files included in this repository that reproduce the results.

1. Download Data -- SQL script to download data from Google BigQuery. (txt)
2. Text Generation -- Import data, train GPT-2 models, and produce generated text. (Python)
3. Embeddings 2D -- Embed text in two dimensional space with Doc2Vec. (Python)
4. Embeddings 50D UMAP -- Embed text in 50 dimensional space with Doc2Vec and reduce dimensionality with UMAP. (Python)
5. Produce Plots -- RMD file to produce plots and tables for paper. (R)

The written report for this project can be found [HERE](https://voices.uchicago.edu/202102macs37000/2021/06/10/1166/).
