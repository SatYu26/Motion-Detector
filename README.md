# Motion- Detector System -OpenCV #
Python/OpenCV script that detect motion on webcam and allow record it to a file and plot a graph for proper Visualization.

## Description ##

### The Process  ###

The trivial idea is to compute the difference between two frames apply a threshold the separate pixels that have changed from the others and then count all the black pixels. Then the average is calculated with this count and the total number of pixels and depending of the ceil the event is triggered or not.

#### Additional informations: ####
* initRecorder: initialise the recorder with an arbitrary codec it can be changed with problems
in the run method no motion can be detected in the first 5 second because it is almost the time needed for the webcam to adjust the focus and the luminosity which imply lot's of changes on the image
* processImage: contains all the images operations applied to the image
* somethingHasMoved: The image iteration to count black pixels is contained in this method

## Requirements ##

* X86, X86_64, ARMv7 or ARMv8 version of Ubuntu 16.04 or Debian 8 (will most likely work on other Linux based operating systems as well)
* Python 3.4 or above 
* Camera or Video file
* [Install OpenCV](https://opencv.org/) or `pip install opencv-python`
* [Install Bokeh library](https://bokeh.pydata.org/en/latest/) or `pip install bokeh`

## Run Motion Detector ##
Clone the repository and run the command `python plotting.py` in the project directory.

#ENJOY!!
