### ❄Video Processing.
     
   1. **🎯Face detection** : 
   I used MediaPipe(open source cross-platform, customizable ML solutions for live and streaming media) for detecting faces in real-time and drawing bboxes around the detected areas in the image.

   2. **🎯Face markers** :
   We make use of Mediapipe's "facemesh" for tracking eyes, mouth opening detection, and head pose estimation.

   3. **🎯Face orientation** : 
   The orienation that the face makes with the assumed axis is noted and orientations are classifed into Straight,right,left,up or down.

   4. **🎯Face Recognition** : 
   The face detected from the face detector is compared with the registered faces(will talk about this below) and if an unknown face is detected, the user is suspected to be cheating. We use "Facenet" model for this purpose.

   5. **🎯Face Spoofing** :
   It is used for finding whether the face is real or a photograph/image from a phone. The anti-spoofing system is implemented by using a pre-trained model with its weights. The models used so far, could be found under models folder.

## ✨Libraries required.
1. PyAudio
2. SpeechRecognition
3. Mediapipe
4. Pillow
5. nltk
6. Keras API.


## ✨How to use.

💥 Clone the repository onto the local machine.

💥 Setup a virtual environment by installing all required packages as specified in requirements.txt

💥 Replace paper.txt with the required question paper.

💥 Run the file main.py 

💥 Register yourself with 5 captures of images.

💥 Proctoring window would open.

💥 After the end of the exam session, press ESC to close the proctoring window and generate reports which would be stored in proctoring_report folder.
