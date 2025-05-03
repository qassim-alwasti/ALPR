# Automatic License Plate Detection and Recognition System (ALPR) for Bahraini License Plates (LP)

## Description:
End to End Deep Learning (DL) pipeline trailored for Bahraini LPs with the following structure:
1. Yolov9e DL model trained from scratch on custome dataset for LP detection.
2. Pretrained Segment Anything Model (SAM) for LP segmentation.
3. A custom LP perspective correction scheme.
4. A custom DL model based on CRNN and CTC loss trained from scratch on custom dataset.

### Code:
The code available under "ALPR\QSM_DemoScript_ALPR_GitHub.ipynb" is the implementation script which is in Python language for the end-to-end pipeline described above. Every part of the code is clearly described and explained. The pretrained models are too large to be added to this github repo and can be shared upon request by emailing "qassim.alwasati@gmail.com". 

### Dataset:
Our cuatom dataset comprises of:
1. LP Detection Dataset in Yolo structure for training and validating the DL model. Only portion of this dataset is added to this repo due to it's large size. It consists of a total of 3000 images (and thier labels) for training and 600 images (and thier labels) for validating the trained DL model.
2. For LP Recognition, a custom dataset of 1000 images are used to train the custom CRNN model and 100 for validation. 



### DL models:
There are 3 deep learning models required for our ALPR script to work:
1. YOLOv9e model (trained from scratch using custom dataset).
2. Segment Anything Model (SAM) pre-trained model.
3. Custom CRNN model in Keras format (trained from scratch using custom dataset).

(SAM) model is developed and published by Meta. Please refer to thier website to download the pre-trained SAM model - below link:
https://segment-anything.com/


## Usage:
1. Make sure you have all the required libraries installed. List of required libraries is in the ipynb script.
2. Download the required DL pre-trained models and place them in the correct path as per the script - you can change it if required.
3. Place the testing dataset in the described path - you can chage it if required.
4. Execute the script to compile the code and execute it. You can run the method "run_ALPR_on_directory(directory)" to perform ALPR on test images avaialble in a specific path.

