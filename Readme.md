# Recognizing Hand Movements Using EEG Signal Classification

## Intro

My graduation project, It's a motor imagery-based brain-computer interface (MI-BCI) application. It's about the classification of different hand movements using the EEG signals of the brain.

Our Project focused on studying the brain signals and their ability to control the movement of the upper limb of the hand and predicting the movement direction from 6 different movements [up, down, right, left, forward, backward] using the EEG signals of the brain through the motor imaginary execution of these movements.


## Paper & Dataset Description

This study provides a large intuitive dataset for 11 different upper extremity movement tasks obtained during multiple recording
sessions. The dataset includes 60-channel electroencephalography, 7-channel electromyography, and 4-channel
electro-oculography of 25 healthy participants collected over 3-day sessions for a total of 82,500 trials across all the
participants.

We only worked on the 6 movements of Arm-Reaching [up, down, right, left, forward, backward].

![image]()


- You can find the paper we worked on at: &nbsp; https://academic.oup.com/gigascience/article/9/10/giaa098/5918864?login=false#supplementary-data
- The dataset can be found at: &nbsp; http://gigadb.org/dataset/view/id/100788/Sample_page/3
- The converted data can be found at: &nbsp; https://ftp.cngb.org/pub/gigadb/pub/10.5524/100001_101000/100788/EEG_ConvertedData/
- The raw data can be found at: &nbsp; https://ftp.cngb.org/pub/gigadb/pub/10.5524/100001_101000/100788/RawData/


## System Architecture

![image]()


## Methodology 

We used 3 different feature extraction techniques:
1. Discrete wavelet transform (DWT)
2. Common Spatial Pattern (CSP)
3. Extracting statistical features


## Classification Methods

We used different machine learning methods such as SVM, Adaboost, Decision Tree, LDA and Random forest.

Also, we used different deep learning architectures such as EEGNET (CNN Architecture), LSTM and different customized CNN architectures.

### EEGNET Architecture :
  
![image]()


## Implementation Results

### For Intra-Subjects

The following Bar chart shows our results when classifying 6 movements for different subjects (`blue`) in comparison with the original Paper (`orange`)

![image]()


### For Cross-Subjects

The following line chart shows how the performance change when changing the number of classes for cross-subject results
    
![image]()


## Deployment 
  
We used Unity to create a simulator that takes the signals for one trial and predicts the direction of movement.

The simulator can be found here: &nbsp; https://drive.google.com/file/d/1mrWMTimOA4dxspdH9cZ9dznV2-6pDoZW/view?usp=sharing

## Demo

![video]()
