# German Traffic Sign Image Classification

This project focuses on classifying images of German traffic signs using Convolutional Neural Networks (CNNs). The dataset contains images of 43 different types of traffic signs, which are preprocessed and fed into a deep learning model for classification. The project includes a full pipeline, from data preprocessing and model training to deployment on a web application.

## Table of Contents
1. [Project Links](#project-links)
2. [Dataset](#dataset)
3. [Installation and Requirements](#installation-and-requirements)
4. [Model Training](#model-training)
5. [Web Application](#web-application)
    - [App Overview](#app-overview)
6. [How to Use](#how-to-use)
7. [Files in This Repository](#files-in-this-repository)
8. [Future Improvements](#future-improvements)
9. [License](#license)

## Project Links

- **Kaggle Notebook:** [German Traffic Sign Image Classification](https://www.kaggle.com/code/hamdipolu/gtsrb-german-traffic-sign-image-classification)
- **Hugging Face Space (Streamlit Web App):** [German Traffic Sign Classification](https://huggingface.co/spaces/poluhamdi/GermanTrafficSignClassifcation)

## Dataset

The dataset used for this project is the [German Traffic Sign Recognition Benchmark (GTSRB)](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset). It contains over 50,000 images of 43 classes of traffic signs.

## Installation and Requirements

To run the project locally, you'll need the following libraries, which are specified in the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

Here are the main dependencies:
- Streamlit
- TensorFlow
- Pillow
- OpenCV
- NumPy

## Model Training

The model is a Convolutional Neural Network (CNN) built with Keras and TensorFlow. After training, the model achieved an accuracy of **92%** on the validation set, demonstrating its effectiveness in classifying traffic signs.

## Web Application

The project is deployed as a web application using Streamlit and hosted on Hugging Face Spaces. Users can upload images of traffic signs, and the model will predict the class of the sign.

To run the web app locally, execute:

```bash
streamlit run app.py
```

### App Overview

The app allows users to upload an image in `jpg`, `jpeg`, or `png` format. After uploading, the model processes the image and predicts the traffic sign class from the 43 categories available. You can see the class labels and predictions displayed within the app interface.

## How to Use

1. Clone the repository.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Run the Streamlit application using `streamlit run app.py`.
4. Upload an image of a traffic sign through the web interface and receive a prediction.

## Files in This Repository

- `app.py`: Contains the code for the Streamlit web application.
- `requirements.txt`: Lists the dependencies required for running the project.
- `GTSRB_model.h5`: Pre-trained model file, which is used in the Streamlit app for traffic sign classification.

## Future Improvements

- **Data Augmentation:** Implement data augmentation techniques to further improve the model's accuracy.
- **Model Optimization:** Experiment with deeper networks and hyperparameter tuning.
- **Deployment:** Explore deployment on other platforms like AWS or Google Cloud.

## License

This project is licensed under the MIT License.
