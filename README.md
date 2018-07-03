# Image Processing of Satellite Images
The main purpose of this project is to identify roas within a satellite image provided by Sentinel-2 which is operated by ESA.
These images are available and are free to use.
We used some elements of image processing and mathematical morphology to recognize the roads and compare the final image to the original.

## Getting Started
To use this project on your images all you have to do is download the .ipynb file which is a jupyter notebook file, and if you don't have it already install the Anaconda Navigator that has the Jupyter Notebook. After opening it just go to directory where you downloaded the file to and open it.

## How to use it

There are two ways to deal with the images, either you can go to a online converter and convert your .jp2 image to a .png image beforehand or use the .jp2 directly. 
In our notebook file we devided the code in blocks for better understading and because to run it we don't need to use everything. 

The first part are the includes that are necessary to run any of the different parts of the code.
After that the first two blocks are parts that we don't actually use for our image in specific. The first of those ones is a function to open a .jp2 file and the following is a generalised version of what we used for our own image that is seen below. This code isn't functional but it was supposed to tranform a big image into 15 smaller images to be able to see in more detail the algorithm working and to take conclusions.

The fourth block is the code used for our image that only works for images that have a dimension of 10980x10980. This images are going to be stored in a folder named "images".

After this we just have to run the two remaining blocks. The first one has the functions that were used to obtain the roads. We used Canny and a mathematical morphology known as dilation.

The next block is the pre-processing we did to the original image. We used a function to enhance the constrast of the image to be easier to apply the other functions to identify the roads.

### Prerequisites

To use everything on the script there is the need to install some packages on Anaconda. They are:

**OpenCV**

```
conda install -c conda-forge opencv
```

**PIL**

```
conda install -c anaconda pillow 
```
**Gdal**

```
conda install -c conda-forge gdal 
```

### Exemples for our Image 
![Example 1](https://github.com/AnnieEm/TA/blob/master/exemplo1.PNG)
![Example 2](https://github.com/AnnieEm/TA/blob/master/exemplo2.PNG)

## Built With
* [Anaconda](https://anaconda.org/)

## Authors

* **Ana Esmeralda Fernandes** - A74321 - [AnnieEm](https://github.com/AnnieEm)
* **André Almeida Gonçalves** - A75625 - [Simbs38](https://github.com/Simbs38)
