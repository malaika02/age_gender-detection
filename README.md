
Age and Gender Detection
Overview
This project uses a Convolutional Neural Network (CNN) implemented with TensorFlow and Keras to detect age and gender from facial images. The model is trained on the UTKFace dataset, which contains a wide variety of faces labeled with age, gender, and ethnicity.

Dataset
The UTKFace dataset contains over 20,000 face images with the following labeling format:

Filename format: age_gender_ethnicity.jpg
age: Integer value representing the age.
gender: Integer value where 0 represents male and 1 represents female.
ethnicity: Not used in this project.


Requirements
Make sure to install the required packages:

bash
Copy code
pip install tensorflow pandas matplotlib scikit-learn
How to Run
Set Up Environment: Ensure you have Python and the required libraries installed.
Prepare the Dataset: Place the UTKFace dataset images in the directory specified by the DATA_DIR variable in the code.
Run the Code: Save the main script as age_gender_detection.py and run it:
bash
Copy code
python age_gender_detection.py
Model Training: The model will train for a specified number of epochs.
Model Saving: After training, the model will be saved as age_gender_detection_model.h5.
Model Architecture
The model is based on the ResNet50 architecture, which is used as a feature extractor.
The output layer has two branches:
Gender output: A binary classification layer (sigmoid activation).
Age output: A regression layer (linear activation).
