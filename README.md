# SCT_ML_3
SVM Cat vs Dog Classifier - Internship Task 3
==============================================

This project implements an SVM (Support Vector Machine) classifier using scikit-learn 
to distinguish between images of cats and dogs. It was developed as part of 
Internship Task 3 at SkillCraft Technology.

----------------------------------------------
📁 Dataset Structure
----------------------------------------------
Ensure your dataset is organized like this:

PetImages/
├── Cat/
│   ├── cat1.jpg
│   ├── cat2.jpg
│   └── ...
├── Dog/
│   ├── dog1.jpg
│   ├── dog2.jpg
│   └── ...

Note: Avoid corrupted images for better training results.

----------------------------------------------
🚀 How It Works
----------------------------------------------
1. svm_train.py
   - Loads images from the Cat and Dog folders.
   - Resizes images to 64x64.
   - Flattens the images.
   - Trains an SVM model using scikit-learn.
   - Saves the trained model as 'svm_cat_dog_model.pkl'.

2. svm_predict.py
   - Loads the saved model.
   - Takes an input image path.
   - Preprocesses the image.
   - Predicts whether the image is a Cat or Dog.
   - Displays the prediction result on the image window.

----------------------------------------------
🛠️ Requirements
----------------------------------------------
Install the required libraries using pip:

pip install numpy opencv-python scikit-learn joblib

----------------------------------------------
🧠 Training the Model
----------------------------------------------
Run the training script:

python svm_train.py

Make sure to update the correct folder paths inside `svm_train.py`:

cat_folder = r"C:\path\to\PetImages\Cat"
dog_folder = r"C:\path\to\PetImages\Dog"

----------------------------------------------
🐾 Predict a Test Image
----------------------------------------------
Run the prediction script:

python svm_predict.py

Edit the test image path in `svm_predict.py`:

test_image = r"C:\path\to\your\image.jpg"

----------------------------------------------
📈 Output
----------------------------------------------
The predicted label ("Cat" or "Dog") will be displayed on the image window.

----------------------------------------------
📌 Notes
----------------------------------------------
- Image size: 64x64
- Input features: raw pixel values
- To improve accuracy further, consider using advanced feature extraction 
  methods or a deep learning model like CNN.

----------------------------------------------
✨ Author
----------------------------------------------
V. Madhan Raj
Machine Learning Intern - SkillCraft Technology
GitHub: https://github.com/madhan90258
