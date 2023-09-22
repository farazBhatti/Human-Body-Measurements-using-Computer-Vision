# Human body measurement using computer vision/ 3D modeling
Anthropometric measurement extraction

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/image_1_50.png)


Getting human body measurements from image is a very hard problem. This repository contains the source code and related files for a system that uses computer vision and 3D modeling techniques to accurately measure various body parts of a human subject.

The system is built on top of the OpenCV and Tensorflow libraries, which provide powerful tools for image processing, feature detection, and 3D reconstruction. It takes single image as input of a human subject and extracts key points. These key points are then used to build a 3D model of the subject, which can be used to precisely measure different body parts such as arm length, waist circumference, and hip width.
This repository provides a starting solution for any one who is working in this domain. All meausrements are in centimeters. 3D reconstruction is done using [HMR](https://github.com/akanazawa/hmr). Tested on tensorflow==1.13.1.

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202021-01-27%2014-34-16.png)

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202023-03-28%2020-12-31.png)

###  Download pre-trained model
Type the following command on terminal to download pretrained model

`wget https://people.eecs.berkeley.edu/~kanazawa/cachedir/hmr/models.tar.gz && tar -xf models.tar.gz`

and save it in 'models' folder.

### CustomBodyPoints

Download [CustomBodyPoints](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/files/5886235/customBodyPoints.txt) text file and place it in data folder.

### Install Packages

   `pip install -r requirements.txt`
   or
   `pip3 install -r requirements.txt`

## Jupyter NoteBook / Quick Demo 
A jupyter notebook has been added for those who quickly want to get inference without much hassel. Simply change path to your input image.
Thanks to [Hamza Khalil](https://github.com/hamzakhalil798) for adding this notebook.

## Inference
`python3 inference.py -i <path to Image1> -ht <height in cm>`
 
## My LinkedIn
[FarazBhatti](https://www.linkedin.com/in/farazahmadbhatti/)

## Acknowledgment
[HMR](https://github.com/akanazawa/hmr)

[Deep lab v3 +](https://github.com/rishizek/tensorflow-deeplab-v3)

[Humanbody shape](https://github.com/1900zyh/3D-Human-Body-Shape)

