# Workplace-security-with-covid-prevention

A system for a workplace environment to prevent the risks of the coronavirus along with the verification of the identity of the employees. we are using OpenCV for face recognition 
that will be projected to the database and is used for verification of the candidate as a legitimate employee, followed by mask detection. Also, on 
entry to the premises, readings are taken using temperature and pulse sensors which are constantly monitored, and alerts via email are sent 
to the personnel department in case the values cross a certain threshold.

Face recognition

There are different steps involved in face recognition. OpenFace and dlib are used to build a face recognition system. The first step is face 
detection. face detection is done using the Histogram of Oriented Gradients(HOG) feature for face detection evaluation.
HОG lооks аt every рixel in the image and forms a gradient.The gradient is 
analysed in lighter to darker pixel.Then we use the face landmark estimation algorithm to generate 68 
specific points (called landmarks) that exist on every face

<img src="https://user-images.githubusercontent.com/75268931/127803124-1c646b33-0a6a-422e-81c3-ef878e64fdd5.png" widht=400 height=400>

The next step is to generate the face encodings for the unknown face we found in with all the pictures we have of people that we already 
know. A deep neural network is used to train it to generate 128 measurements for each face. These are called encoding. After 
generating the encoding these are matched with the image that we generated.

Face Mask Detection

The face mask detection is developed with a machine learning algorithm through image classification. The First step is face 
detection. For face detection viola jones algorithm is used. The Viola-Jones algorithm first detects the face on the grayscale image and then 
finds the location on the colored image.It searches for haar-like features which are used to find the faces. It detects 3 haar-like features 
including edge features, line features, four-sided features.


<img src="https://user-images.githubusercontent.com/75268931/127803311-bdada01c-bbe4-46a3-9ef0-330fa447b9b8.png" widht=400 height=400>

Health Monitoring

The system is set up by using an Arduino UNO board, along with LM35 temperature sensor and a pulse sensor connected to it. Along 
with it an LCD display is connected, so that the values of the temperature and pulse rate are visible on the physical setup as well. 
The code added to the Arduino is such that ,the a certain threshold value is set, upon crossing which alerts are generated.



<img src="https://user-images.githubusercontent.com/75268931/127803517-bd2d8c96-a4f6-49ff-b447-53ea10e55855.png" widht=400 height=400>


