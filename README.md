# Human body measurement using computer vision/ 3D modeling
Anthropometric measurement extraction

![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/img1.png)


Getting human body measurements from image is a very hard problem. This repository provides a starting solution for any one who is working in this domain.
It maps single input image onto 3-dimientional model using 3D human reconstruction and then extracts body measurements such as waist, chest etc. All meausrements are in centimeters. 3D reconstruction is done using [HMR](https://github.com/akanazawa/hmr) .
![alt text](https://github.com/farazBhatti/Human-Body-Measurements-using-Computer-Vision/blob/master/sample_data/input/Screenshot%20from%202021-01-27%2014-34-16.png)



## Inference
`python3 inference.py -i <path to Image1> -ht <height in cm>`

 
