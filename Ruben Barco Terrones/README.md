# Multi-modal Local and Recurrent Non-verbal Emotion Recognition in Dyadic Scenarios

This folder contains the repository of the master thesis of **Rubén Barco Terrones** in relation with the **Non-acted Multi-view Audio-Visual Dyadic Interactions Project**.

### Description of the Master Thesis
This Master Thesis is focused on the development of baseline **emotion recognition system** in a dyadic environment using raw and handcraft audio features and cropped faces from the videos. This system is analyzed at frame and utterance level with and without temporal information. For this reason, an exhaustive study of the state-of-the-art on emotion recognition techniques has been conducted, paying particular attention on Deep Learning techniques for emotion recognition.

While studying the state-of-the-art from the theoretical point of view, a dataset consisting of videos of sessions of dyadic interactions between individuals in different scenarios has been recorded. Different attributes were captured and labelled from these videos: body pose, hand pose, emotion, age, gender, etc. Once the architectures for emotion recognition have been trained with other dataset, a proof of concept is done with this new database in order to extract conclusions. In addition, this database can help future systems to achieve better results.

A large number of experiments with audio and video are performed to create the emotion recognition system. The **IEMOCAP database** is used to perform the training and evaluation experiments of the emotion recognition system. Once the audio and video are trained separately with two different architectures, a fusion of both methods is done. In this work, the importance of preprocessing data (i.e. face detection, windows analysis length, handcrafted features, etc.) and choosing the correct parameters for the architectures (i.e. network depth, fusion, etc.) has been demonstrated and studied, while some experiments to study the influence of the temporal information are performed using some recurrent models for the spatio-temporal utterance level recognition of emotion.

### Repository Explanation

All the scripts are coded in Python and tested and debugged using Spyder (Anaconda). The paths inside the codes vary between the perosnal paths of my computer and the paths of the server provides by **HuPBA** (Human Pose Recovery and Behavior Analysis). Normally, all the training and preprocessing files should have the paths from the server because they are computationally expensive. 

The repository is organized in the following way: 

* **Dockerfiles**: the two dockerfiles coded for runing the experiments on the server:
  * hola
* **Preprocessing**: all the scripts coded for organizing the IEMOCAP database, for the preprocessing of audio, features and video and for creating all the .txt, .csv and dictionaries for the training process.
* **Emotion Recognition**: all the training scripts for the Emotion Recognition system used in the master thesis.
