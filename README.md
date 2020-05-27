# Saihiel Bakshi's Data Science Portfolio
Welcome! This is a portfolio curated of some of the cool projects that I have worked on. Feel free to contact me if you have any questions!

# [Project 1: Generating News Headlines](https://github.com/saihiel/news_headlines)
Writing a good news headline is an art. It requires a strong command over language to be able to grab the readers attention in a single sentence. In this project I created a model that takes an orginal news headline and generates a related but new one.
This project focuses on the application of **deep learning to natural language processing**. I worked with a subset of Reuters news headlines that are collected over 15 months.
* Built an autoencoder where the encoder and decoder networks consist of recurrent neural networks trained using teacher forcing.
* Implemented data augmentation for improving the robustness of the autoencoder, as proposed by Shen et al [[1]](https://arxiv.org/pdf/1905.12777.pdf).
* Analysed the embedding space of headlines by interpolating between headlines.
* Developed a system to extract the most similar headlines to a given headline.  
An interesting example of the project's success:
   Original Headline: Wall street rises, limps across the finish line of a turbulent year.
   Generated Headline: Wall street rises after the losses from the markets poor performing year.
What's interesting about this sample is that it demonstrates the models ability to infer the meaning of the headline within the context and generate a new one with the same meaning!
*Keywords: Deep Learning, Natural Language Processing, Autoencoder, Recurrent Neural Network, Data Augmentation, Interpolation*


# [Project 2: Classifying Pairs of Shoes for the Visually Impaired](https://github.com/saihiel/Classifying-Shoe-Pairs)
Have you ever looked at two shoes and wondered whether they come from the same pair or not? Me neither. But unfortunately, not everyone has this privledge. People with visual impairments face similar challenges daily. In this project I designed and developed a model that can function as the underlying model for a system that deals with this issue.  
This end-to-end project deals with preprocessing the image data, creating models with two different convolutional architectures, training the neural networks (including tuning hyperparameters) and evaluating the models. 
* Cleaned and preprocessed image data using numpy and created visualizations using matplotlib
* Built two *convolutional neural networks* using pytorch, each with different architectures
* Tuned the hyperparameters for each model varying learning rate, dropout, weight decay, learning rate decay, batch size and the number of feature maps to find the optimal combination of capacity, speed, and generalization for my models.

Since the characteristics of mens and womens shoes are different, I evaluated my model's performance seperately on mens shoes and womens shoes.
Learning Curve for Model 1:
![](https://github.com/saihiel/Data-Portfolio/blob/master/images/Project2/model%201%20learning%20curve.png)
Learning Curve for Model 2:
![](https://github.com/saihiel/Data-Portfolio/blob/master/images/Project2/model%202%20learning%20curve.png)
Model 2 acheived a higher validation accuracy and was hence selected to be evaluated on the test set. The model achieved  an accuracy of **85%** on womens shoes and **76%** on mens shoes. I suspect this difference is due to more defining characteristics commonly present on womens shoes.
An example of mens shoes classified correctly:
![](https://github.com/saihiel/Data-Portfolio/blob/master/images/Project2/mens_correct.png)
An example of womens shoes classified incorrectly:
![](https://github.com/saihiel/Data-Portfolio/blob/master/images/Project2/womens_wrong.png)
