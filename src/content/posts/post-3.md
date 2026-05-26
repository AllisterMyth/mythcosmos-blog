---
title: "I made a Cancer Prediction model"
date: 2026-05-24T05:00:00Z
image: /images/B1.jpg
categories:
  -  BioMaths
  - Machine Intelligence
draft: false
---

I’ve been really big into cancer research using machine intelligence lately. It all started when I heard about the man who cured his dog of cancer using AI. In short he scanned all the DNA abnormalities that the cancer cells had and made custom medicine that taught body’s army, the immune system to identify all cells with these particular abnormalities as enemies. If you want more details, I will put a link at the end. Now I was very inspired to create something that actually helped in any form in cancer research. As I later realised, that thought was much too naive. 

The biggest issue or so I thought in the beginning was which model to choose. At first I made a model that took regular blood tests and flagged any abnormal pattern using Gradient Boosted Trees but that was too simple and started underfitting. The main constraint was feature extraction as in defining features which are essentially just mathematical functions to get more value from raw data. Problem is it’s hard to notice real features on a small dataset without knowing biology. I tried teaching myself more about cancer markers in blood biopsy but ultimately gave up due to inefficiency. It was taking more time for me to understand biology than to understand machine learning. I felt moving to a more ML heavy problem might be optimal.

As I searched for a new problem statement, I learnt a lot more about general ML models and theories. Here I came to know about the two biggest constraints, Data and Compute. I realised that making a model or rather choosing a model was the easy bit. The hard part was training the model on good data and reducing the compute used. It turns out that good datasets related to cancer were relatively low on sites like Kaggle and the best database was NIH cancer db. Even on NIH cancer db you would need certain permissions which you can only get as a ML researcher. During my hunt, I came across Sybil AI by MIT. It was a CNN ResNet model that predicted cancer risk in the next few years with above 80% accuracy. It was trained on a big NLHS db on NIH. It only took CT scan images and a lot had changed since when it was made in Jan 2023. 

I finally found my problem; I wanted to make a model that would predict future cancer risk like Sybil but unlike sybil would take blood biopsy, diagnosis along with CT scans as input which would in theory boost the accuracy and detection rate. I used a Resnet-Swin tiny hybrid with pretrained weights for CT scan and retrained Clinical BERT for reading diagnosis. A gated method is used for multimodal fusion which essentially decides by itself which model’s decision making would be prioritised for what kind of patient. I trained the model on a small synthetic dataset made from NLHS db. Unlike Sybil, this model can work for any specific type of cancer if trained on relative data. I truly hope this model becomes something useful even if just as an inspiration for you or me to develop further models on. Although for now it serves as more of a proof of concept than a usable model. 

Thank you for giving me your time and have a nice day.

Allister Myth


Check out my project: https://github.com/AllisterMyth/Multimodal-Cancer-Prediction.git
The man who cured his dog: https://www.forbes.com/sites/johnwerner/2026/04/05/he-solved-his-dogs-cancer-three-ai-models-helped/