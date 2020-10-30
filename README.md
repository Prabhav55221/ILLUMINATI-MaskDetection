# Team ILLUMINATI - Myntra HackerRamp
## Component 2 - Face Mask Detection
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

For our complete submisisson, headover to - https://github.com/swatig23/myntra_ILLUMINATI
This is the second component of our project - *Real Time Face Mask Detection (RM - FMD)*

Before going further please see the demo - ____Insert Video____

# Features!

  - Easy 5 step setup on your local PC.
  - Interactive WebApp that supports upload of images upto 200 MB for processing.
  - We don't want to brag, but our model achieves over 99.3% accuracy and can identify *tricks* like - "Hand Covering Face", "Imperfect Mask" and "Towels coverign face".

You can also:
  - Use this as an API!
  - Use your webcam and/or an external camera for mask detection using our Command Line Arguements.


# Tech

Our RM-FMD uses a number of open source projects and libraries to work properly:

* Tensorflow - For training our DL Model.
* Keras - For helping us evaluate our DL Model
* Open CV - For Face Recognition and all our computer vision needs.
* Caffe - A deep learning framework made with expression, speed, and modularity in mind. Used for Face Detection.
* Mobile Net V2 - Pretrained DL Model
* Streamlit - Open Source Project that helps us serve our models as a web app.

# Installation

We have tried to keep the installation process as simple as possible. Please keep note of the following points:

* Please follow the exact steps.The App is tested and verified only if each step is followed.
* First time deployment of app might take 1 -2 minutes.
* Note that all commands are to be entered with Admin Permissions in the command line.

Step 1 - Clone the Repository.
```sh
$ git clone https://github.com/Prabhav55221/ILLUMINATI-MaskDetection.git
$ cd ILLUMINATI-MaskDetection
```

Step 2 - Create Virtual Env and Download Reqs.
```sh
$ mkvirtualenv tester
$ pip3 install -r requirements.txt
OR
$ mkvirtualenv tester
$ pip install -r requirements.txt
```

And that's it! You are done. Let's now get this working.

# Working

##### Web Application Mode

Step 1: CD into the folder
Step 2: Run the server and enjoy!

__Note that the Website does not support Webcam mode due to deployment issues.__

```sh
$ cd ILLUMINATI-MaskDetection
$ streamlit run app.py
```

##### API Mode - For all you devs out there

Step 1: CD into the folder
Step 2: Now you can use both __PHOTO__ and __WEBCAM MODE__ by entering the following code

> Image Mode (Pass any image using the --image flag.)
```sh
$ python3 detect_mask_image.py --image images/pic1.jpeg
OR
$ python detect_mask_image.py --image images/pic1.jpeg
```

> Website Mode
```sh
$ python3 detect_mask_video.py 
OR
$ python3 detect_mask_video.py 
```

# That's it !

Team Illuminati
NSUT, Delhi
