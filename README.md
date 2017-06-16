# Human-Detection From a Image

# Deep Learning

# Overview
Introduces an approach for Human detection in an image with sliding window. 
The Idea behind this approach is to train a CNN model on images which we want to detect.
After that make a sliding window on the image and query the trained model to produce appropriate output. 

# Dependencies
This project requires Anaconda  Python 3.5  and the following Python libraries installed:
* tensorflow
* tflearn
* h5py
* hdf5
* SciPy
# Note: For Windows
Run this if you did not create environment using anaconda gui.
```
conda create -n my_env python=3.5  
conda install -c conda-forge tensorflow
 pip install tflearn
 ```
 ##### Implementation
 
 ## Model 
 
 # Layers
  1. Conv: 64 filters of size 3x3 with ReLU activation
  2. Pooling: with filter size 2x2
  3. Conv: 32 filters of size 3x3 with ReLU activation
  4. Pooling: with filter size 2x2
  5. Conv: 32 filters of size 3x3 with ReLU activation
  6. Pooling: with filter size 2x2
  7. Fully Connected: with 256 neurons and ReLU activation and dropout with probability 0.5
  8. Fully Connected: with 256 neurons and ReLU activation and dropout with probability 0.5
  9. Fully Connected output layer: with 2 neurons (equal to number of classes) and softmax classifier.
 

 
 # Train Dataset
 Create a Data set frome a video. Capture a video from any Enviroment where humans or non hymans.
 you can get picture frome video by crop the single human or non human only pic
 you can crop picture by matlab code 
 * Image_crop_video.m
 Save picture in Data folder which have two other folder give name like 0 or 1
 * 0 contain humans pictures
 * 1 contains nonhumans pictures
 * give path of Data folder in code
  # Test Dataset
   It like just train  data set make video and get pictures frome it like 10 to 15 nonhuman or human 
   and test the data from it
 # human pic like this

![11](https://user-images.githubusercontent.com/27928395/27203084-9c48dacc-523d-11e7-8d28-ec83d0636429.jpg)

 # Nonhuman pic like this
 ![11](https://user-images.githubusercontent.com/27928395/27203047-75651376-523d-11e7-85f8-f892c8b38c4f.jpg)
 
 # Training
 Run this file in your cmd enviroment 
 Python Train.py
 
 # Testing
 Run this file in your cmd enviroment 
 Python Test.py
 
 # Result
 # Traning data Screen shot
 ![train](https://user-images.githubusercontent.com/27928395/27202983-30fc0b18-523d-11e7-9ede-be669e3e1595.png)
 
 # Test  data screen shot
 ![test](https://user-images.githubusercontent.com/27928395/27203021-58888850-523d-11e7-9bb6-ec1cec32f165.png)
 
 ### Discussion 
 I thoroughly studied the approach for human detection butt the best one is Convolutional Neural Networks in Deep learning 
 Because it took time to figure out the result but the results of this algorithm is accurate 99%
 
