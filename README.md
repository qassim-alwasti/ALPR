# ALPR
A pre-trained deep learning models for Automatic License Plate Detection and Recognition (ALPR) specifically for Bahraini License Plates

There are 3 pre-trained models required for our ALPR script to work:
1. YOLOv9e pre-trained model.
2. Segment Anything Model (SAM).
3. Custom pre-trained CRNN model in Keras format.

(SAM) model is developed and published by Meta. Please refer to thier website to download the pre-trained SAM model - below link:
https://segment-anything.com/

The pre-trained YOLOv9e model and custom CRNN model can be found in this repo. 
We also added Python script in "ipynb" format which is used to run our end-to-end ALPR system.
In "TestImages" folder, there are 19 images of cars with Bahraini License Plates downloaded from "www.platesmania.com" which can be used to test the code. 
