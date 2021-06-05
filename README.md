# Rock_paper_scissor

The whole game is divided into three steps :
1. Data collection
2. Creating model
3. Creating final game interface

## Data collection:
- First we created a region of interest (ROI) , the image inside that box is only captured
- Using OpenCV , we collected the indivisual images of hand gestures of Stone , paper and scissor

## Creating model
- first from our direcory , we loaded our data set of images
- then resize them to (112 ,112)
- Using train_test_split , we split the data into labels and their respective sign gesture
- For model creation , we use CNN (convolutional neural network) 
- for image classification , we build the sequential model which consist of four Convo2D layers , 3 dense layer and a flatten layer.
- this model is inspired from a pretrained model of keras-image classificaion ie *VGG16* , our model is just  a small part of it.

## Final game interface

- finally on our openCV screen , we created two box (one for user move , other one for computer's move)
- both moves and result gets printed on screen
