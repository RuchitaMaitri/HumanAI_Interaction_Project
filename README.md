# Using AI for Accessibility
This project is created by Ruchita Maitri for the course 05-318 Human AI-Interation Course at Carnegie Mellon University.


## This is a preliminary attempt to develop an android application to help people with visual impairment navigate better!

People with visual impairment find it difficult to carry out their daily activities. With time they do get used to their surroundings. However, navigating outside comfortable space remains a challenge. This necessitates a one stop solution which can describe the surrounding for visually impaired people in an effective manner. Live surrounding captioning would be ideal. With this motivation in my mind, I decided to develop an android applicationt to predict the traffic light color in (almost) real-time to give output in an audio format. For the purpose of this academic project, due to limited time and resources, I have kept the scope very limited. 

### Collecting data:
There are plenty of resources available which capture traffic related image data for developing self-driving cars. For this project I have used super-clean data from Udacity's Intro to Self-Driving Car course project (Link in the resources section). This data has approximately 1500 images of traffic signal lights red, yellow and green. Yellow signal data is very limited, close to only ~100 images. This has definitely affected model's prediction capacity for this class.

### Model Development:
This has been treated as an image-classification model with 3 classes, 'Red', 'Yellow', and 'Green'. For developing image classification model, I used Teachable Machine by Google. Teachable Machine is a web based tool that makes creating machine learning model super fast and easy. Teachable Machine uses MobileNet model to classify image. 

### Android Application Development:
To use this developed model, Teachable Machine provides Tensorflow-Lite version which can be used in Android application development. I further used a Text-To-Speech functionality within Android Studio to generate the audio output. I referred to the starter code in the resource section and referred to the tutorial (linked in resources) to understand how to add image capturing functionality, how to add tensorflow-lite model in the back-end. I added code (on my own) to manipulate the predicted class probabilities to display appropriate text on the app and pass on to Text-To-Speech API. 

Final application can be run by simply downloading the .apk file on the android device. 

You can download the .apk file to test it out! 

### Resources
- https://github.com/kobbled/ITSDC-Udacity-Traffic-Light-Classifier
- https://www.youtube.com/watch?v=jhGm4KDafKU
- https://gist.github.com/ishaanjav/8575a9c0a21ee59273137d7ba1de1727
- https://gist.github.com/ishaanjav/4fe84d57d1ca4f887fbfe220dfa504c3



