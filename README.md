# FaceMaskDetector
This CNN model is trained to identify if a person is wearing a mask or not.

Dataset Used -
https://www.kaggle.com/andrewmvd/face-mask-detection
~ The above dataset contains 853 images belonging to 3 classes: with mask, withput mask and incorrect mask

About the model -
This model implements VGG16 as the main framework for training the model with the datasets. 
~ Sequential model
~ Dropout (0.3) used to prevent the model from overfitting the data
~ 2 Dense layers with ReLU and Sigmoid as activation functions
~ Compiled using 'binary_crossentropy' as loss function

How we increased accuracy -
~ Tried different values for dropout to get the best one
~ Chose a better dataset as the one chosen primarily had multiple copies of images and photoshopped ones.

Training after 20 epochs - 
loss: 1.5964e-04 - accuracy: 1.0000 - val_loss: 0.0440 - val_accuracy: 0.9899
