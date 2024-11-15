# Human body measurement using computer vision/ 3D modeling
Anthropometric measurement extraction

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/image_1_50.png)



Accurately obtaining human body measurements from a single image is a challenging task. This repository provides the source code and associated files for a system that leverages computer vision and 3D modeling techniques to achieve precise body part measurements.

The system utilizes OpenCV and TensorFlow for advanced image processing, keypoint detection, and 3D reconstruction. By analyzing a single image of a human subject, it identifies key points and reconstructs a 3D model. This model enables accurate measurements of various body parts, including arm length, waist circumference, and hip width, with results provided in centimeters.

Built on top of the [HMR](https://github.com/akanazawa/hmr) model, this solution serves as a robust starting point for researchers and developers working in this domain. The code has been tested with TensorFlow 1.13.1 for compatibility and reliability.


![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202021-01-27%2014-34-16.png)

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202023-03-28%2020-12-31.png)

###  Download pre-trained model
Type the following command on the terminal to download pre-trained model

`wget https://people.eecs.berkeley.edu/~kanazawa/cachedir/hmr/models.tar.gz && tar -xf models.tar.gz`

and save it in 'models' folder.

### CustomBodyPoints

Download [CustomBodyPoints](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/files/5886235/customBodyPoints.txt) text file and place it in the data folder.

### Install Packages

   `pip install -r requirements.txt`
   or
   `pip3 install -r requirements.txt`

## Jupyter NoteBook / Quick Demo 
A Jupyter notebook has been added and updated for those who quickly want to get inference without much hassle. Simply change the path to your input image.
Thanks to [Hamza Khalil](https://github.com/hamzakhalil798) for adding this notebook.

## Inference
`python3 inference.py -i <path to Image1> -ht <height in cm>`
 
## My LinkedIn
[FarazBhatti](https://www.linkedin.com/in/farazahmadbhatti/)

## Acknowledgment
[HMR](https://github.com/akanazawa/hmr)

[Remove_background](https://github.com/farazBhatti/bg_remove_GUI)

[Deep lab v3 +](https://github.com/rishizek/tensorflow-deeplab-v3)

[Humanbody shape](https://github.com/1900zyh/3D-Human-Body-Shape)

