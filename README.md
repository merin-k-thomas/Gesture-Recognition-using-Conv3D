# Gesture-Recognition-using-Conv3D
A gesture recognition model for smart televisions that can recognise five different gestures performed by the user which will help users control the TV without using a remote will be developed. . The architecture used to process videos is the 3D convolutional neural network. 

The gestures are continuously monitored by the webcam mounted on the TV. Following gestures are considered for the modelling:
1.	Thumbs up:  Increase the volume
2.	Thumbs down: Decrease the volume
3.	Left swipe: 'Jump' backwards 10 seconds
4.	Right swipe: 'Jump' forward 10 seconds  
5.	Stop: Pause the movie

The training data consists of 663 videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). The videos have two types of dimensions - either 360x360 or 120x160. And the validation data consists of 663 videos categorised into one of the five classes. For analysing videos using neural networks, the 3D convolutional network is used. 

In 3D Convolutional Networks or Conv3D, convolution and pooling operations are performed spatio-temporally. In this case, the input to a 3D conv is a video (which is a sequence of 30 RGB images). The video becomes a 4-D tensor of shape l x h x w x c, where c is the number of channels, l is length in number of frames, h and w are the height and width of the frame, respectively. Also, 3D convolution and pooling kernel size are referred by d x k x k, where d is kernel temporal depth and k is kernel spatial size. In 3D convolutions, the filter convolves in three directions. Thus, the output shape after performing a 3D conv with one filter is a 4-D tensor.
