# Face-recognition-using-JavaScript
Face detection is one of the most common applications of Artificial Intelligence. The use of Facial detection has increased in the last couple of years.  Face-api.js has brought a JavaScript API for face detection and face recognition in the browser implemented on top of the tensorflow.js core API.
Step1 - Create a folder called face-recognition

Under the face-recognition folder create the following folder structure.

All folders are self-explanatory except models. That I will cover in going forward.

Step2 - download the face-api.min.js

Download the face-api.min.js code from the following URL and paste it inside the js/face-api.min.js file.


https://github.com/MOHINIM19/
Step3 - download the modal files

Models are the trained data that we will use to detect the feature from the face.

Download the files from the following URL and placed them inside the models folder.

https://github.com/MOHINIM19

Step4 - Let's built the index.html file.

In index.html file we importing the style.css for styles, face-api.min.js for processing the model data and extracting the features and main.js where we will write our logic.

Inside the body tag we are creating a video tag to get the face, result-container for showing the emotion, gender, and age.

Place the below code inside the index.html file okayStep5 - Let's built the main.js file.

Inside the main.js file we are using promise.all to load the models to the face API. once the promise is resolved then we are calling the startVideo method that starts the streaming. Below are the methods used for this demo

faceapi.detectSingleFace method - detectSingleFace utilize the SSD Mobilenet V1 Face Detector. You can specify the face detector by passing the corresponding options object. To detect the multiple faces replace the detectSingleFace with detectAllFaces

withFaceLandmarks method - It is used for Detecting 68 Face Landmark Points

withFaceExpressions method - This method Detect all faces in an image + recognize facial expressions of each face and return the array

withAgeAndGendermethod - This method Detect all faces in an image + estimate age and recognize gender of each face and return the array.

Step6 - Let's Add the style to the app.

Replace the style.css 

Step7 - Let's run the app by the live server or http-server.

