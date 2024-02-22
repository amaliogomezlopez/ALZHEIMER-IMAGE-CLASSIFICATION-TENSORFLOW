
# 📑ALZHEIMER IMAGE CLASSIFCATION
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)


![Python](https://img.shields.io/badge/Python-100000?style=flat&logo=python&logoColor=FFFFFF&labelColor=5C5C5C&color=3776AB)
![Numpy](https://img.shields.io/badge/NumPy-100000?style=flat&logo=Numpy&logoColor=FFFFFF&labelColor=5C5C5C&color=013243)
![Pandas](https://img.shields.io/badge/Pandas-100000?style=flat&logo=Pandas&logoColor=FFFFFF&labelColor=5C5C5C&color=150458)
![MatPlotLib](https://img.shields.io/badge/MatPlotLib-100000?style=flat&logo=LOT-Polish-Airlines&logoColor=FFFFFF&labelColor=5C5C5C&color=E4637C)
![Plotly](https://img.shields.io/badge/Plotly-100000?style=flat&logo=Plotly&logoColor=FFFFFF&labelColor=5C5C5C&color=3F4F75)
![Jupyter](https://img.shields.io/badge/Jupyter-100000?style=flat&logo=Jupyter&logoColor=FFFFFF&labelColor=5C5C5C&color=F37626)
![postgresql](https://img.shields.io/badge/SQL-100000?style=flat&logo=postgresql&logoColor=FFFFFF&labelColor=5C5C5C&color=CC2927)


This project is based on the following dataset:  https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset

The data consists of MRI images. The data has four classes of images both in training as well as a testing set:

- Mild Demented
- Moderate Demented
- Non Demented
- Very Mild Demented
The data contains two folders. One of them is augmented ones and the other one is originals.
Originals could be used for validation or test dataset…

Data is augmented from an existing dataset.

The original data is the one that I am going to use for the test at the end.

# PROJECT WORKFLOW

# Loading the data

- In this step the define the paths for the augmented data and original data

- Target Distribution: 4 Categories:
![Images Loaded](https://i.postimg.cc/h43ShXym/cerebros.png)




# Split the data

- We use ImageDataGenerator and flow_from_drectory to split the data in:

- TRAIN: 27188 images belonging to 4 classes.
- VALIDATION: 6796 images belonging to 4 classes.


# Model 

I used Sequential model. We can check the model's architecture here: 
![Model Architecture](https://i.postimg.cc/mZqyjSpg/model-architecture.png)

# Evaluation

![Metrica Accuracy & Loss](https://i.postimg.cc/Hkck8NHN/acc-loss.png)
![ROC AUC](https://i.postimg.cc/WzZPbB0m/auc.png)


- Decreasing Loss: The training loss and validation loss are both decreasing over the epochs. This indicates that the model is learning and improving its ability to make predictions.

- Increasing Accuracy: The training accuracy and validation accuracy are both increasing over the epochs. This suggests that the model is becoming more accurate in classifying the data.

- Performance Discrepancy: In some epochs, there is a slight discrepancy between training and validation performance. For example, in Epoch 7, there is a higher validation loss and lower accuracy compared to the training set. This could be due to overfitting or issues in the data distribution. I need to monitor this and consider applying regularization or adjusting the model architecture if necessary.

- High Validation Accuracy:The validation accuracy reaches a high value of around 99.12% in the last epoch, indicating that the model generalizes well to unseen data.

- Consistent Improvement: The model continues to improve over the epochs, with decreasing loss and increasing accuracy. This is a positive sign of effective learning.

- ROC AUC: AUC on the training set also improves, suggesting that the model is getting better at distinguishing between positive and negative instances. The AUC on the validation set is consistently high, indicating that the model performs well in terms of classification ability.

# CONTACT
[Amalio Gómez](https://amaliogomezlopez.com/)

[![GitHub Followers](https://img.shields.io/github/followers/amaliogomezlopez?style=social)](https://github.com/amaliogomezlopez)  
[![LinkedIn Connect](https://img.shields.io/badge/LinkedIn-Connect-blue?style=social&logo=linkedin)](https://www.linkedin.com/in/amaliogomezlopez/)
