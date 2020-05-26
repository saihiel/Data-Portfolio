# Saihiel Bakshi's Data Science Portfolio
A portfolio of my data science projects for which the code can be made publicly available. The project are not in a particular order. The goal of my portfolio is for each project to demonstrate a certain interest of mine, while also showcasing some of my work.

# [Project 1: Generating News Headlines](https://github.com/saihiel/news_headlines)
Writing a good news headline is an art. It requires a strong command over language to be able to grab the readers attention in a single sentence. In this project I created a model to generate a new and different news headlines from a given headline.  
This project focuses on the application of **deep learning to natural language processing**. I worked with a subset of Reuters news headlines that are collected over 15 months.
* Built an autoencoder where the encoder and decoder networks consist of recurrent neural networks trained using teacher forcing.
* Implemented data augmentation for improving the robustness of the autoencoder, as proposed by Shen et al [1](https://arxiv.org/pdf/1905.12777.pdf).
* Analysed the embedding space of headlines by interpolating between headlines.
* Developed a system to extract the most similar headlines to a given headline.  
*Keywords: Deep Learning, Natural Language Processing, Autoencoder, Recurrent Neural Network, Data Augmentation, Interpolation*
