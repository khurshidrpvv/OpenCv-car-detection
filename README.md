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
