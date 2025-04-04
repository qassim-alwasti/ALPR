# ALPR
Deep learning models trained on custom dataset for Automatic License Plate Detection and Recognition (ALPR) specifically for Bahraini License Plates

There are 3 deep learning models required for our ALPR script to work:
1. YOLOv9e model (trained from scratch using custom dataset).
2. Segment Anything Model (SAM) pre-trained model.
3. Custom CRNN model in Keras format (trained from scratch using custom dataset).

(SAM) model is developed and published by Meta. Please refer to thier website to download the pre-trained SAM model - below link:
https://segment-anything.com/

We also added Python script in "ipynb" format which is used to run our end-to-end ALPR system.
