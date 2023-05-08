# Multispeaker Lipsync with Speaker Diarization 

This repository contains the code and resources for our project titled "Multispeaker Lipsync with Speaker Diarization" submitted as a part of our Bachelor's Degree in Computer Science and Engineering at the National Institute of Technology, Tiruchirappalli.

## Introduction
With the increasing demand for video content in multiple languages, dubbing has become a common practice to cater to a wider audience. However, the lip-sync issues that arise during the dubbing process often lead to a poor viewing experience. Automating the lip-sync process can significantly reduce the manual labor involved in dubbing.

In this project, we propose a speaker and language-independent lip-sync model that accurately synchronizes lips with audio. The model uses a speaker diarization and face recognition module to identify the speaker in each frame and perform lip-sync only for that specific speaker.

We utilized the following libraries and models in our project:

* Wav2Lip for generating realistic lip movements based on audio
* GFPGAN for generating high-quality face images from low-quality inputs
* Pyanote.audio for speaker diarization and face recognition

## Model Architecture
The proposed model architecture consists of a speaker diarization module which tells us who speaks when further this data is passesd to our face detection and recognition once the face is identified into the frame the lipsyncronization is applied after genereating these lip movements we apply super resolution to make it more smooth. It includes a speaker diarization module that identifies the speaker in each frame and a GAN that generates lip movements based on the audio input.

## Result and Analysis

## Usage
To run the code, please follow these steps:

Clone this repository
1. Run the speaker_diarization.ipynb to obtain transcript
2. Run the Wav2Lip-GFPGAN.ipynb for final results

# Acknowledgments
We would like to express our sincere gratitude to our project guide, Dr. M. Sridevi, for her valuable guidance and support throughout this final year project. We also thank to Dr. Sriram for his invaluable advice and assistance during the course of this project. We are grateful to the evaluation panel for their time and effort in reviewing our project and providing us with constructive feedback. Finally, we thank Dr. G. Aghila for giving us this opportunity. 
