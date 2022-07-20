# Diabetic-Retinopathy-Detection
Detecting diabetic retinopathy utilizing convolutional neural networks through image-classification

# Diabetic Retinopathy
Diabetic Retinopathy is an eye disease that is part of the greater diabetes diagnosis. It is a complication of diabetes, where high blood-sugar can block blood vessels from transferring blood, damaging the vessels and subsequently lead to blindness and/or glaucoma.

# Initial Thought Process
For starters, TensorFlow is a free and open-source Pythonic library for machine learning analysis. In addition, Keras is an open-source library that provides a Pythonic interface for libraries like TensorFlow. Both work together to create work. I decided to create a program in Python that can essentially classify, to a large extent, whether the images shown to it is a normal, healthy eye, or an eye with moderate Diabetic Retinopathy. For an opthalmologist, it can be fairly straightforward for the doctor to check the condition of the eye, but it is a completely different matter when it comes to the computer. Thus, I decided to create an experiment on whether it can accurately detect diabetic retinopathy.

# The Details
I used one of the more popular and accurate class of neural networks called Convolutional Neural Networks (CNN, for short) to implement this testset (3 Conv2D models and 2 MaxPooling2D models, to be specific). With my samples, I divided them up into 3 files to be trained on ("train," "validation," and "test"), each separately either a normal batch of pictures, or moderate diabetic retinopathy. With 15 epochs, the program was able to get to near 95% accuracy with regards to the samples. I used mathplotlib to plot the results.

# Confounding Variables
The sample size was very small (2000 images in total), so overfitting was easy to do for the computer (the machine-learned pictures are far too close to the pictures used to train the models).

# Future improvements
1. Greatly increase the sample size of the pictures
2. Add dropout and data augmentation to increase accuracy, incase of less sample size in general
3. Utilize pre-trained models such as the Xception model to greatly enhance the accuracy
4. Add more variables, such as severe diabetic retinopathy or proliferated diabetic retinopathy

# Special Thanks To:
-Deep Learning with Python, Francois Chollet
-Sovit Ranjan Rath, Kaggle Datasets
