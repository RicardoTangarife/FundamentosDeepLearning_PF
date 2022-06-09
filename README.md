# Fundamentals of Deep Learning Final Project

For the final project of the Fundamentals of Deep Learning course, we propose to develop initial machine learning models to support our master's research work, which is involved in a project that aims to support the field of public safety, specifically through acoustic and visual signals.
Thus, we generate two models, one for the classification of two sound events and another one for the detection of fights through videos, which support the field of public safety.

A descriptive video of the project can be found at: https://youtu.be/f1YiQp1GbhA

# Sound Classification

To classify sound events, a public dataset of urban acoustic events named UrbanSound8k was selected. This dataset contains 10 different classes of sounds from which 2 of interest for citizen security were chosen, namely the sound of gunshots (gun_shot) and the sound of sirens (siren).

Some samples of the data, displaying for each class its time waveform and frequency spectrogram are as shown below.

![image](https://user-images.githubusercontent.com/36963665/172217337-24b7c4c6-7538-4f83-9602-c7c4eb0c4fed.png)


To see a brief overview of the training process, the historical loss and accuracy of the model in training and test are plotted.
![image](https://user-images.githubusercontent.com/36963665/172218262-0dae9d4f-68a7-44b9-b35c-5be5eaa8e095.png)

In this case, a model based on 2-dimensional convolutional layers was defined to extract these feature patterns from each of the class samples, represented in the intensity values of Mel's ceptral coefficients in frequency. 

Some of the previous studies worked with this dataset can be found in the following section of Kaggle. From there we take some of the suggestions for implementation
https://www.kaggle.com/datasets/chrisfilo/urbansound8k


### Dataset UrbanSound8k

The UrbanSound8k dataset is a public dataset with 8730 tagged sounds, used in different open tasks in kaggle, its disk size is approximately 7GB and the sound files are in .wav format; the class distribution is as follows:

0 = air_conditioner = 873<br>
1 = car_horn = 873<br>
2 = children_playing = 873<br>
3 = dog_bark = 873<br>
4 = drilling = 873<br>
5 = engine_idling = 873<br>
6 = gun_shot = 873<br>
7 = jackhammer = 873<br>
8 = siren = 873<br>
9 = street_music = 873<br>

To access and download this dataset you must go to the official contributors page hosted at the following url:
https://urbansounddataset.weebly.com/urbansound8k.html


# Video Classification

### Dataset UBI-Fights


