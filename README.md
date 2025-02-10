# **Speech Understanding Programming Assignment - 1**

## **Overview**
This repository contains the implementation for Speech Understanding Programming Assignment - 1, covering the following tasks:

--- 

### **Q1: Emotion Recognition Using Wav2Vec2**

**Task Description:**
 - The goal of this task is to perform Emotion Recognition using the RAVDESS dataset and a Wav2Vec2 pre-trained model. This model processes audio speech signals and classifies emotions.

**Dataset Used:**
 - RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
 - Downloaded and extracted using Python.

**Model & Training Details:**
 - Model Used: Wav2Vec2 (pre-trained on emotion recognition)

**Preprocessing:**
 - Convert audio to mono
 - Resample to 16kHz
 - Extract features using Wav2Vec2 processor

**Training:**
 - Optimizer: SGD (learning rate = 1e-3, momentum = 0.9)
 - Loss Function: Categorical Crossentropy
 - 30 epochs
 - GPU-accelerated training

**Results:**
 - Final Test Accuracy: 76.7%

**Classification Report:**
 - Precision: Varies across emotions (highest for Angry & Disgust)
 - Recall: Higher for Neutral & Surprised emotions

### **Q2 Task A: Spectrogram Analysis with Different Windowing Techniques**

**Task Description**

**This task involves:**
 -  the UrbanSound8K dataset.
 - Applying STFT (Short-Time Fourier Transform) to extract spectrograms.
 - Comparing Hann, Hamming, and Rectangular windows to analyze spectrogram differences.
 - Training an SVM classifier to classify sound events based on extracted spectrogram features.

**Dataset Used:**
 - UrbanSound8K(Managed using the soundata library).

**Implementation Details**
  - Feature Extraction:
  - Compute STFT-based spectrograms for different windows.
  - Extract MFCCs (Mel-Frequency Cepstral Coefficients).

**Classifier:**
  - Model: SVM (Support Vector Machine)

**Test Accuracy:** 73.3%

### **Q2 Task B: Music Genre Spectrogram Comparison**

**Task Description**

 - Select 4 songs from 4 different genres and generate spectrograms for each song.
 - Compare frequency distribution, energy levels, and structure.

### **Genres & Songs Used**
| Genre  | Song |
|--------|--------------------------------------------------|
| **Metal**  | Slaughter To Prevail - Baba Yaga |
| **Rock**   | Linkin Park - Numb |
| **Pop**    | Sabrina Carpenter - Espresso |
| **EDM**    | Martin Garrix - Forbidden Voices |


### **Analysis & Observations**
| Genre  | Frequency Distribution | Energy Concentration | Harmonic Content | Structure |
|--------|------------------------|---------------------|-----------------|-----------|
| **Metal**  | High-frequencies dominant | Intense & unstructured | Distorted harmonics | Less structured |
| **Rock**   | Balanced mid-high range | Moderate energy | Clear instrument separation | More structured |
| **Pop**    | Dominant mid-range | Strong in vocals & beats | Well-defined harmonics | Structured rhythm |
| **EDM**    | Strong low/high frequencies | High bass energy | Synthesized harmonics | Highly structured |

## **Installation Instructions**

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/rishi02102017/SpeechUnderstanding_PA1.git
cd SpeechUnderstanding_PA1
```
### **Step 2: Install Dependencies**
 - Make sure you have Python installed. Then, run:
```bash
pip install -r requirements.txt
```
### **Step 3: Run the Scripts**
 - Run the individual scripts as per the sections above.

## **References**

 - UrbanSound8K Dataset: [Salamon et al., 2014]
 - Librosa Library: [McFee et al., 2015]
 - PyTorch: [Paszke et al., 2019]
 - Wav2Vec2: [Baevski et al., 2020]
 - Adam Optimizer: [Kingma & Ba, 2015]

## **Author**

 - Jyotishman Das (M24CSA013)
 - Course: Speech Understanding
 - Institution: Indian Institute of Technology Jodhpur


