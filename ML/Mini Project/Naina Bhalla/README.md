# Mini-Project: Hand Gesture Recognition
### Naina Bhalla

## Overview<br>
The project implements two different models for static and dynamic hand gesture classification. The static model is a NN while the dynamic model is 2D-CNN+LSTM. The final result is shown using cv2 on the webcam-feed.

## Dataset<br>
The static dataset contains 7 classes [one,peace,three,not in dataset,thumbs_up,thumps_down,palm] each with 300 images except "not in dataset" with 500 images of other random gestures. The dyanmic dataset contains of video-frames of 4 classes[wave,clap,no,hand wave] in form of numpy arrays.

## Static Classification<br>
The static model is a neural network trained on the 21 landmarks acquired by mediapipe.<br>

### Model Architecture<br>
![alt text]({2F8E0747-5E19-4EC0-8DCE-BCA2538378E6}.png)<br>

### Accuracy<br>
This achieves test loss of 0.2819 and test accuracy of 93.26%<br>
![alt text](image.png)<br>

## Dynamic Classification<br>
This model is a CNN+LSTM model with TimeDistributed that is used to apply convolutional layers to each video frame independently for sequential learning of the model.<br>

### Model Architecture<br>
![alt text]({F7E30A6C-A66B-4DE9-99EA-8D6F4B571634}.png)<br>
