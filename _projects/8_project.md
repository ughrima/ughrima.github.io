---

layout: page
title: Music Genre Detection
description: Classifying music genres using the GTZAN dataset with machine learning and neural networks.
img: assets/img/spectogram.png
category: Machine Learning
---

This project involves the classification of music genres using the GTZAN dataset. Various machine learning algorithms and neural networks are employed to achieve the best accuracy.

### Dataset
The dataset used is the GTZAN Music Genre Classification Dataset, containing audio tracks categorized into different genres.

### Project Overview
- **Data Cleaning and Preprocessing**: Handled missing values, encoded labels, and normalized the data.
- **Data Visualization**: Visualized waveforms of each genre to understand data distribution.
- **Model Training and Evaluation**: Trained and evaluated several machine learning models:
  - Logistic Regression: 52.33%
  - K-Nearest Neighbors (KNN): 70.67%
  - Decision Tree: 62.00%
  - Random Forest: 78.00%
  - CatBoost: 83.33%
  - XGBoost: 77.33%

- **Neural Network Implementation**: Trained a neural network for 100 epochs, achieving a test accuracy of 75%.

- **Model Comparison**: Compared all models based on accuracy. The CatBoost Classifier performed the best with an accuracy of 83.33%.

### Model Saving and Loading
The best performing model, CatBoost Classifier, was saved using `pickle` for later use:

```python
import pickle as pkl

# Saving the model
with open('cbc_model.pkl', 'wb') as file:
    pkl.dump(cbc, file)

# Loading the model
with open('cbc_model.pkl', 'rb') as file:
    cbc_pkl = pkl.load(file)

# Predicting with the loaded model
predictions = cbc_pkl.predict(x_test)
```

### Key Insights
- **Spectrograms**: Used to visualize audio frequencies over time, providing more information for neural network training.
- **Convolutional Neural Networks (CNNs)**: Leveraged for their efficiency in pattern recognition within spectrograms, improving genre classification accuracy.


### GitHub Repository
Explore the source code and contribute to the project on GitHub:
<a href="https://github.com/ughrima/music-genre-recommendation" class="btn btn-primary" target="_blank">View on GitHub</a>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/spectogram.png" title="Spectrogram Sample" class="img-fluid rounded z-depth-1" %}
    </div>
        <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/s.png" title="Spectrogram Sample" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example spectrogram image of reggae and rock music used for training the CNN model.
</div>

### Libraries Used
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **CatBoost**
- **XGBoost**
- **TensorFlow**
- **librosa**

