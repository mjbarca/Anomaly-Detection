# Anomaly-Detection
This repository contains the public material generated for the master's thesis related to the anomalies detection in in-house devices. The code has been generated in python using Google Colab as a development tool. The content is as follows:
Notebooks:
- RoomsView.ipynb --> load data and shows room data
- DataStudy.ipynb --> load data and makes a study of data. Makes as well data preprocessing to generate models. generate scaled data already preprocesed
- LSTM_model.ipynb --> generates LSTM model from preprocesed data
- AnomalyDetection_mono.ipynb --> detects anomalies from data in a monovariable scenario
- AnomalyDetection_multi.ipynb --> detects anomalies from data in a multivariable scenario

Data has been are collect from https://www.kaggle.com/datasets/ranakrc/smart-building-system. This dataset is collected from 255 sensor time series, instrumented in 51 rooms in 4 floors of the Sutardja Dai Hall(SDH) at UC Berkeley. 

The normal way to perform the notebooks is 

01.- RoomsView for having a plot for each variable and room. It is important to having an idea about data.  
02.- DataStudy Seep insight about data. firstly general and after by room. This notebook generates the dataset with data preprocesated: scaled_KETY.  
03.- LSTM_model load scaled_KETI and performs a model by variable. models are serialized and saved in pickle files.  
04.- AnomalyDetection_mono run models predictions to rooms in order to identify anomalies. Uses pickle files and scaled_KETI data.  
05.- AnomalyDetection_multi generate models for multivariable scenarios and run models predictions to rooms in order to identify anomalies.  

