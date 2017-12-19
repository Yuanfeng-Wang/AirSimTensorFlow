<img src="airsim.png">

This repository contains Python scripts showing how you can use Microsoft AirSim to collect image data
from a moving vehicle, then use that data to train a deep-learning neural net in TensorFlow.  

# Prerequisites

* [Recommended hardware](https://wiki.unrealengine.com/Recommended_Hardware) for running UnrealEngine4, required
for AirSim.  Although it is possible build AirSim on OS X and Linux, we found
it easiest to use the pre-compiled binaries in the
[Neighborhood](https://github.com/Microsoft/AirSim/releases/download/v1.1.7/Neighbourhood.zip)
example.

* [Python3](https://www.python.org/ftp/python/3.6.3/python-3.6.3-amd64.exe) for 64-bit Windows

* [TensorFlow](https://www.tensorflow.org/install/install_windows). To run TensorFlow on your GPU as we and
most people do, you'll need to follow the 
[directions](https://www.tensorflow.org/install/install_windows#[TensorFlow](https://www.tensorflow.org/install/install_windows) for installing CUDA and CuDNN.  We recommend setting aside at least an hour to make sure you do this right.

# Instructions

1. Clone this repository.
2. Download and unzip the [Neighborhood](https://github.com/Microsoft/AirSim/releases/download/v1.1.7/Neighbourhood.zip)
example, open it, and click <b>run.bat</b> to launch AirSim.
3. When prompted, go with the default car simulation.
4. From the repository, run the <b>image_collection.py</b> script.  It will start the car moving and stop 

# Future work

Our single-layer logistic regression network provides a simple proof-of-concept example; however,
for a more realistic data set involving collisions with different types of objects, a 
convolutional network would be more realistic.

# Credits

This code represents the combined work of two teams in Prof. Simon D. Levy's fall 2017 AI course 
([CSCI 315](http://home.wlu.edu/~levys/courses/csci315f2017/)) at 
Washington and Lee University (listed alphabetically):

* Jack Baird 
* Alex Cantrell 
* Keith Denning 
* Rajwol Joshi
* Will McMurtry 
* Jacob Rosen


