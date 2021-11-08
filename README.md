## Yolo-V5-using-Roboflow

**Yolo** is a regression based algorithm. Its full form - You Only Look Once.

This Algorithm divides objects into grid cells wherein each cell is in the grid is responsible for detecting the objects within it. This algorithm is famous for its speed and accuracy.
yoloV5.png

In this following project we are identifying the crop diseased leaves using YoloV5(object detection)

Here we load the labelled images using the link of roboflow. Roboflow makes the image conversions, rotations easy so that we can train our model effeciently.

After loading the data(images) it creates images folder and validation folder.
Images folder has train and test data

#### start the training process
Model is trained for 100 epochs. The time taken for training depends on the number of images and number of steps

After training the weights are dumped into the runs folder.

We use tensorboard to view the graphs of the model training.

### Using the trained weights to run inference on the images

Once any disesed leaf image is given as an input our model runs the weight files and predicts the type of disease and gives o/p with bounding boxes.
