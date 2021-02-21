# Text_to_Speech
A combination of Deep Learning and Google Translate to convert handwritten text to audio output.



This project takes OCR and handwritten text as input and provides translated output in audio format available in 108 different languages.
The backbone of the project is the handwritten text detection model which is trained using transfer learning on RESNET50.


![](Result%20Images/Handwritten/Handwritten%20text%20detection.PNG)




The input for the model was combined from a dataset available on [Kaggle](https://www.kaggle.com/sachinpatel21/az-handwritten-alphabets-in-csv-format) with the MNIST dataset and all the images were resized to (32,32) . The total image count on which model was trained was 4,42,451 .

The model was trained for 50 epochs on SGD optimizer and training and validation accuracy of 96.53% and 96.81% respectively were recorded.

![](training%20plot.png)

The classification report for every character:


![](Classification%20Report.PNG)

The model was trained on Tensorflow 2.1.0 and OpenCV 4.2.0. 

The trained model file is available on [https://github.com/sanskar-hasija/Text_to_Speech/blob/main/Trained%20Model/model.h5](https://github.com/sanskar-hasija/Text_to_Speech/blob/main/Trained%20Model/model.h5)
