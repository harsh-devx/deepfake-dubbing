# Multispeaker Lipsync with Speaker Diarization

This repository contains the code and resources for our project titled **Multispeaker Lipsync with Speaker Diarization** submitted by **Harsh Khandelwal**, **Advai Swamy** and **Dhruv Kachhadia** as a part of our Bachelor's Degree in Computer Science and Engineering at the National Institute of Technology, Tiruchirappalli.

## Introduction

In this project, we propose a one shot speaker and language-independent lip-sync model that accurately synchronizes lips with audio when there are multiple faces in the frame which the original model doesn't handle. The model uses a speaker diarization and face recognition module to identify the speaker in each frame and perform lip-sync only for that specific speaker.

We utilized the following libraries and models in our project:

- Wav2Lip for generating realistic lip movements based on audio
- GFPGAN for generating high-quality face images from low-quality inputs
- Pyanote.audio for speaker diarization and face recognition

## Model Architecture

The proposed model architecture consists of a speaker diarization module which tells us who speaks when. This data is then passesd to the face detection and recognition module. Once the face is identified in the frame, lip synchronization is applied after generating these lip movements. We apply super resolution to improve the quality of the lip synced face. It includes a speaker diarization module that identifies the speaker in from the audio clip and a GAN that generates lip movements based on the audio input.

![](img/Proposed%20methodology.png)

## Usage

To run the code, please follow these steps:

Clone this repository

1. Run the speaker_diarization.ipynb to obtain transcript
2. Run the Wav2Lip-GFPGAN.ipynb for final results

# Acknowledgments

We would like to express our sincere gratitude to our project guide, **Dr. M. Sridevi**, for her valuable guidance and support throughout this final year project. We also thank to **Dr. Sriram** for his invaluable advice and assistance during the course of this project. We are grateful to the evaluation panel for their time and effort in reviewing our project and providing us with constructive feedback. Finally, we thank Dr. G. Aghila for giving us this opportunity.
