# OpenCv car detection

## Descripton:

Much of the unstructured data that exists today and will be created in the future is image or video data. Instagram, Facebook, CCTV etc.Our project will demonstrate how to detect vehicles from a CCTV image using a cascade of boosted classifiers based on HAAR like features.We are going to train our har cascade to detect cars.

## Dependencies
[Python](https://www.continuum.io/downloads)

[OpenCv](http://opencv.org/) or it can be downloaded `pip install opencv-python`

## Training Harcascade:
To train har cascade first we need to have cropped images of object of interset(Positive images) and object that are not of our interest(Negative Image).

In our cas positive images consist of cars and negative images consist of images that do not have cars.Ideally negative images should be something that is related to the envionment of positives.So our negatives have roads images.

Dataset used for training can be downloaded from [Vehivle Image database](http://www.gti.ssr.upm.es/data/Vehicle_database.html)

To train harcascade we need three different files,that we have to create:

  **1. Positive Description file** 
  
  These files contains the information about all the positive images. Foramt of this file is `full_path+image_Name+Number_Of_PositiveObject_in_Image+x coordinat+ y coordinate+width+Height` This is used with `-info` flag.See the `info.txt` for more clarification.
  
  **2. Negative Description file**
  
  This file contains inforamtion about the Negative images. Format for this file is `full_path+image_name`.It is used with `-bg` flag,where bg stands for background. See `bg.txt`
  
  **3. Vec file**
  
  This file contains the inforamtion of positive images in binary,it is used in har training.It is used with `-vec` flag.In our case `cars.vec` is the required vector file.
  
  HarTraining folder has the step by step guide to create these files and train har.
  
