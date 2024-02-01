# Augmented PIN Authentication Through Behavioral Biometrics

This code package is related to the paper:

M. Nerini, E. Favarelli, and M. Chiani, "[Augmented PIN Authentication through Behavioral Biometrics](https://www.mdpi.com/1424-8220/22/13/4857)," Sensors, 2022.

If you use this code or any modified part of it, please cite our paper.

## Abstract

Personal Identification Numbers (PINs) are widely used today for user authentication on mobile devices. However, this authentication method can be subject to several attacks such as phishing, smudge, and side-channel. In this paper, we increase the security of PIN-based authentication by considering behavioral biometrics, specifically the smartphone movements typical of each user. To this end, we propose a method based on anomaly detection that is capable of recognizing whether the PIN is inserted by the smartphone owner or by an attacker. This decision is taken according to the smartphone movements, which are recorded during the PIN insertion through the built-in motion sensors. For each digit in the PIN, an anomaly score is computed using Machine Learning (ML) techniques. Subsequently, these scores are combined to obtain the final decision metric. Numerical results show that our authentication method can achieve an Equal Error Rate (EER) as low as 5% in the case of 4-digit PINs, and 4% in the case of 6-digit PINs. Considering a reduced training set, composed of solely 50 samples, the EER only slightly worsens, reaching 6%. The practicality of our approach is further confirmed by the low processing time required, on the order of fractions of milliseconds.

## Content of Code Package

The `dataset` folder contains 12 datasets obtained by 12 different students. Each dataset is a .txt file representing a 470 x 17 matrix in which:

* each row is a sampled digit.
* each column is a feature: the first is the pressed digit and the following are motion sensor values.

The `PIN_authentication.ipynb` Jupiter Notebook contains the code to replicate the results in the paper.

The files `rocMat.mat` and `times.mat` have been obtained throguh `PIN_authentication.ipynb` and are attached for an easier replication of the figures.
