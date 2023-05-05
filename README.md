# Semantic-Segmentation-FCN-32-model
Semantic segmentation classifies image pixels into one or more classes which are semantically interpret able. CNNs for semantic segmentation typically use a fully convolutional network (FCN) architecture, which replaces the fully connected layers of a traditional CNN with convolutional layers.  

## Overview
Semantic Segmentation is an image analysis task in which we classify each pixel in the image into a class.
So, let's say we have the following image.

![](https://lh3.googleusercontent.com/-ELUnFgFJqUU/XPPXOOmhfMI/AAAAAAAAAP0/2cabsTI9uGUYxM3O3w4EOxjR_iJvEQAvACK8BGAs/s374/index3.png)

And then given the above image its semantically segmentated image would be the following

![](https://lh3.googleusercontent.com/-gdUavPeOxdg/XPPXQngAnvI/AAAAAAAAAQA/yoksBterCGQGt-lv3aX4kfyMUDXTar7yACK8BGAs/s374/index4.png)

As you can see, that each pixel in the image is classified to its respective class.


# Results

![image](/results/horse.png)


## Properties of Segmentation Model:

Semantic segmentation aims to identify each pixel in the input image with the appropriate class that represents a particular item. The Fully Convolutional Network (FCN), which stacks several convolutional layers with comparable padding to retain dimension, is one method for segmentation.

Convolution: A segmented map is produced by the model's several convolutional layers, which extract information from an input picture of any size.

Pooling: The resolution of complicated features is decreased by pooling, which also lowers the computing load. This aids in lowering noise levels while obtaining dominant features.

Upsampling: increases the input image's resolution, allowing the algorithm to produce more precise predictions.

Skip Connections: A FCN's resolution is decreased by downsampling, and when it is upsampled, producing fine details is challenging. Thus, skip connections provide the layers enough data to construct more precise segmentation borders or accurate spatial organization.

Evaluation Metric(IOU) for Segmentation Model:

The Jaccard Index, or IOU, is calculated by dividing the area of union between the anticipated segmentation and the ground truth by the amount of overlap between the two. IOU has a range of 0 to 1, with 0 denoting no overlap and 1 denoting flawless overlap segmentation.

The mean IOU of the picture is determined for binary or multi-class segmentation by averaging the IOU of each class.

# Folder Structure
```
📦Semantic-Segmentation-FCN-32-model
 ┣ 📂results
 ┃ ┣ 📜horse.png
 ┃ ┣ 📜sem_seg.png
 ┃ ┗ 📜sem_seg_inf.png
 ┣ 📜.gitignore
 ┣ 📜LICENSE
 ┣ 📜README.md
 ┗ 📜semantic_segmentation_fcn32.ipynb
```