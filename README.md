# TrafficSignClassfication_CovNet
Classification of Traffic signs images data set using Convolution neural network Using the LeNet architecture . 
The data set was obtained form here - https://bitbucket.org/jadslim/german-traffic-signs.
The contents are signnames.csv  test.p  train.p	valid.p, the pickle files were depicked and the 'features' and 'labels' were extracted 
Since in traffic signs the color has has nothing much to do all the images were converted into greyscale and cv2.equalizeHist(img) was used 
for histogram equalisation with increases the contrast with would help in feature extraction.
The model had 2 convolutional layers with 60 (5,5) fitlers in the  and 
2 more convolutional layers with 30 (3,3) filters ,it has 2 maxPooling layers of size (2,2) with a stride of 1 and no padding .
It also has 2 dropout layer with a droupout of 50% .
The model was tested using a image of a sign obtained form here - https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/STOP_sign.jpg/220px-STOP_sign.jpg
and was found to classify it right with an accuracy of 96 %
The accuracy can further be increased using data augmentation upto 99%
