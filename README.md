# FaceMaskDetector

TRAINING CODE: First thing the given dataset is very small, the original dataset which I used in the given program contains 1,980 images of both labels i.e with mask and without mask and I downloaded it from kaggle but github doesn't allow to upload more than a 100 files, so I deleted many images and kept only 50 for both labels.
In the attached code I've used deep learning for training the model to predict Face Mask in real time but instead of convolutional layer I've used MobileNet as it is much faster than convolutional layer and uses less parameters making code easy to understand and after that I've done max pooling and flattening and then the fully connected layer and then saved the model in h5 format...


TEST CODE: In the test code first i've created a function in which i've taken 3 parameters as input which are frame (frames which are going to be captured in real time by our webcam), Facenet (Caffemodel due to which we will detect the face) and Masknet (Our trained moedel which will predict whether mask is there or not).So, instead of usiing opencv for face detection or haarcascade frontal face algorithm, I've used caffemodel so that the code'll be less bulky...
