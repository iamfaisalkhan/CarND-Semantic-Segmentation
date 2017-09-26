# Semantic Segmentation

[//]: # (Image References)
[image1]: ./figs/um_000000.png
[image2]: ./figs/um_lane_000000.png
[image3]: ./figs/um_000003.png
[image4]: ./figs/um_000004.png
[image5]: ./figs/um_000005.png


### Introduction
In this project, we segment roads in [Kitti](http://www.cvlibs.net/download.php?file=data_road.zip dataset using Fully Convolutional Network (FCN).

### Training

#### Dataset 

The kitti dataset contains images of roads with multiple level of labeling. We used the training consist of images of the following form:

![][image1]

The ground truth is provided as a labeled pixels seperating background from the road segment in the image:

![][image2]


#### Network

We implemented the FCN8 network from the [paper](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Long_Fully_Convolutional_Networks_2015_CVPR_paper.html) using tensorflow.

### Results

The network was trained using Adam optimizer for 10 EPOCHs using a batch size of single image. Here is a sample of results:

![][image3]
![][image4]
![][image5]


