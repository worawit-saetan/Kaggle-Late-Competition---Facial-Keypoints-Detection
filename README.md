# Kaggle Late Competition - Facial Keypoints Detection
Detect the location of keypoints on face images

## Outline is as follows
+ load the data set and check
+ delete images which have incomplete information (missing some y columns)
+ turn image string value into numeric value

+ split train/ validation /test set

+ normalize the data by dividing 255.0

+ reshape the image data and add repeat channel axis

+ do the data augmentation

+ download Mobilenet as a model base and create our own custom on top of that

+ freeze base model and train (feature extraction)

+ plot model metric and val matric (RMSE)

+ fine tune the model by unfreezing some based layers and train our model with decreasing learning rate

+ plot model metric and val matric (RMSE)

+ evaluate the model with test set

+ save the model

+ use our model to predict the kaggle test data

+ create the submission file 

+ due to some prediction values that exceeds the constraint range of 0-96 (pixels), we edit these values with maximum value (96)
