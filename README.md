# Text_to_Speech
A combination of Deep Learning and Google Translate to convert handwritten text to audio output
![](Result%20Images/Handwritten/Handwritten%20text%20detection.PNG)


This project takes OCR and handwritten text as input and provides translated output in audio format available in 108 different languages.
The backbone of the project is the handwritten text detection model which is trained using transfer learning using RESNET50.

The input for the model was combined from a dataset available on [Kaggle](https://www.kaggle.com/sachinpatel21/az-handwritten-alphabets-in-csv-format) with the MNIST dataset and all the images were resized to (32,32) . The total image count on which model was trained was 4,42,451 

The model was trained for 50 epochs on SGD optimizer and training accuracy and validation accuracy of 96.53% and 96.81% respectively were recorded.

![](training%20plot.png)
