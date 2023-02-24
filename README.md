![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)

# Concrete Crack Images Classification
 To identify whether the picture is positif crack or negative crack

## Data loading
- code using Google Colab
- download the dataset with the following code

```
!wget https://prod-dcd-datasets-cache-zipfiles.s3.eu-west-1.amazonaws.com/5y9wdsg2zt-2.zip

!unzip "5y9wdsg2zt-2.zip" 
!unrar x "Concrete Crack Images for Classification.rar"
```

## Feature selection
- get the negative and positive path image as feature
- set positive and negative as target 

`ref = {0:'positive', 1:'negative'}`

## Data preprocessing
### read and resize images
- read the image as grey color and resize to a much smaller resolution (50,50)
- set the x and y dimension
- train test split

## Model development
- using sequential and activation softmax as output

![img](/model.png)

![img](/model_training.png)

## Callbacks
 - set tensorboard and early stopping to prevent overfitting
 - set the epoch to 5 and batch size at 16
 - train the model
 
 ## Model analysis
 ![img](/model_analysis.png)
 ![img](/accuracy.png)
 
 ## Model prediction
 - L is the label image
 - P is the predicted images
 - it shows all the prediction images is correct
 
 ![img](/predicted_image.png)
 
 ## Model deployment
 - save the model in h5 format

## Acknowledgement
- [Özgenel, Çağlar Fırat (2019), “Concrete Crack Images for Classification”, Mendeley Data, V2, doi: 10.17632/5y9wdsg2zt.2](https://data.mendeley.com/datasets/5y9wdsg2zt/2)

