# face_recog using-opencv
Libraries used are- cv2,imutils,numpy,pickle
from sklearn.preprocessing import LabelEncoder
from sklearn.svm import SVC

We have performed face recognition with opencv using a pre-trained OpenFace model along with built-in opencv libraries which are.prototxt and .caffe models for detection of the faces.Deep neural network(dnn) module with Caffe model is used for face detection.

We are also making use of cv2.dnn.blobFromImage which performs following functions:
1.Mean subtraction
2.Scaling/Normalising
3.Optionally channel swapping.

Adding dataset to the datapath.Appending the images to the respective filename
Creating empty face_embeddings and face_names and processing the images. Using blobfromimage above functions will be performed.
The .prototxt file defines the model architecture.The .caffemodel file contains the weights for the actual layers based on these models face embeddings are created and appended to the empty list to quantify a face.
Fix a threshold value and here we are giving 50%, if the datasets has many images we can set the threshold value to 30% still it will recognise the face.

Drawing the rectangle around face.We can give input as image file or using webcam.Thus,face is recognised using opencv with better accuracy. 

