# Human body measurement using computer vision/ 3D modeling
Anthropometric measurement extraction

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/img1.png)


Getting human body measurements from image is a very hard problem. This repository provides a starting solution for any one who is working in this domain.
It maps single input image onto 3-dimientional model using 3D human reconstruction and then extracts body measurements such as waist, chest etc. All meausrements are in centimeters. 3D reconstruction is done using [HMR](https://github.com/akanazawa/hmr). Tested on tensorflow==1.13.1.

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202021-01-27%2014-34-16.png)



## Inference
1. Download the pre-trained models.
Type the following command on terminal

`wget https://people.eecs.berkeley.edu/~kanazawa/cachedir/hmr/models.tar.gz && tar -xf models.tar.gz`

and save it in 'models' folder.

2. Download [CustomBodyPoints](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/files/5886235/customBodyPoints.txt) text file and place it in data(make new one) folder.


3. Install packages
   `pip install -r requirements.txt`
   or
   `pip3 install -r requirements.txt`

4. Run inference
`python3 inference.py -i <path to Image1> -ht <height in cm>`
 
## Acknowledgment
[HMR](https://github.com/akanazawa/hmr)

[Deep lab v3 +](https://github.com/rishizek/tensorflow-deeplab-v3)

[Humanbody shape](https://github.com/1900zyh/3D-Human-Body-Shape)
