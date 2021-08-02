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



The next step is to generate the face encodings for the unknown face we found in with all the pictures we have of people that we already 
know. A deep neural network is used to train it to generate 128 measurements for each face. These are called encoding. After 
generating the encoding these are matched with the image that we generated.
