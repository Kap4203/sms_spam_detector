# SMS Spam Detector

## Overview
This project is an SMS Spam Detection application that uses a machine learning model to classify SMS messages as either "spam" or "not spam". It utilizes a pipeline that includes TF-IDF vectorization and a Linear Support Vector Classification (SVC) model to make predictions.


## Files and Directory Structure
```
├── sms_spam_detector/
    ├── sms_text_classification_solution.ipynb
    ├── gradio_sms_text_classification.ipynb
    ├── Resources/
        └── SMSSpamCollection.csv
    ├── README.md
    └── LICENSE
```
- **sms_text_classification_solution.ipynb**: Jupyter notebook with the solution for SMS text classification.
- **gradio_sms_text_classification.ipynb**: Jupyter notebook containing the Gradio interface to interact with the classification model.
- **Resources/SMSSpamCollection.csv**: Dataset containing SMS messages labeled as "spam" or "ham" (not spam).
- **README.md**: Documentation for the project.
- **LICENSE**: License information for the project.

## Dependencies
- **Python 3**
- **pandas**: For data manipulation library.
- **scikit-learn**: Machine learning library for building the model.
- **gradio**: Library for creating the user interface.


## How It Works
1. **Data Loading**: The dataset (`SMSSpamCollection.csv`) is loaded using pandas.
2. **Preprocessing and Model Training**: The SMS messages are transformed using TF-IDF vectorization, and a Linear SVC model is trained to classify the messages.
3. **Prediction Function**: A function called `sms_prediction` is created to classify incoming SMS messages using the trained model.
4. **Interactive Interface**: Gradio is used to create an interface where users can input SMS text and get a prediction of whether it is spam or not.

### Notes
If you want to create a public link to share your app, use share=True in the launch() method.
By default, running sms_app.launch() will launch the app locally.

## Dataset
The dataset used in this project (SMSSpamCollection.csv) contains labeled SMS messages, with labels "ham" indicating not spam, and "spam" indicating spam. This dataset is used to train the machine learning model.

## License
This project is licensed under the Unlicense. See the LICENSE file for more information.

## Author
David Kaplan