# Augmented PIN Authentication Through Behavioral Biometrics

This code package is related to the paper:

M. Nerini, E. Favarelli, and M. Chiani, "[Augmented PIN Authentication through Behavioral Biometrics](https://www.mdpi.com/1424-8220/22/13/4857)," Sensors, 2022.

## Content of Code Package

The `dataset` folder contains 12 datasets obtained by 12 different students. Each dataset is a .txt file representing a 470 x 17 matrix in which:

* each row is a sampled digit.
* each column is a feature: the first is the pressed digit and the following are motion sensor values.

The `PIN_authentication.ipynb` Jupiter Notebook contains the code to replicate the results in the paper.

The files `rocMat.mat` and `times.mat` have been obtained throguh `PIN_authentication.ipynb` and are attached for an easier replication of the figures.
