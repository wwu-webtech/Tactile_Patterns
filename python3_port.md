#How to port to python 3:

## How does it work?:

The program will grayscale the image, increase contrast, making a map over the image depending on given saliency parameters, and based on this making a high contrast black and white. From here, the images can be printed and ran through a heating apparatus that gives texture based on whether a section is white or black, giving a sensory indication of features of an image or map, allowing for it to help viusally impaired people. The heating apparatus and paper can be found within OM 360 of WWU.

## How to install and run the program through the CLI:

1. Install python: Installing python from [Here](https://www.python.org/downloads). For this tutorial, version, v3.10.11 was used.

2. Make sure that python and pip are both installed correctly and the correct version with 'python --version' and 'pip --version'. python version 3.11.10 and pip version 24.3.1 were used for this projects developement.

3. These two libraries allow for cv2 commands to continue to be used in python 3:
   '''
   pip install opencv-contrib-python
   pip install argsparse
   '''
   If these are not added to PATH, do so on windows using the System Enviornment Variables in windows. A sussinct guide can be found [here](https://linuxize.com/post/how-to-add-directory-to-path-in-linux/) for adding variables to path for linux and mac.

In testing, installing these two dependencies allowed the retention of all functionality of the cli, as opencv retains support of cv2 functions.

4. run the following command from the tactile_imaging folder:
   'python tactile_patterns\photo2tactile.py -i tactile_patterns\photos\input.jpg -o tactile_patterns\output'
   where input.jpg is whatever photo you wish to run through the system. NOTE: it doesn's have to be a jpg image type.
