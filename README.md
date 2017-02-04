## What does this repository contain?

This repository contains 13 class labels for both train and test dataset in NYUv2. This is to avoid any hassle involved in parsing the data from the .mat files. If you are looking to train a network to do 13 class segmentation from RGB data, then this repository can provide you both the training/test dataset as well the corresponding ground truth labels. However, if your networks needs additionally depth data (either depth image or DHA features) then you will need to download the dataset from the [NYUv2 website](http://horatio.cs.nyu.edu/mit/silberman/nyu_depth_v2/nyu_depth_v2_labeled.mat) (~2.8GB) as well as the corresponding [toolbox](http://cs.nyu.edu/~silberman/code/toolbox_nyu_depth_v2.zip). To summarise, this repository contains the following

- The **train_labels_13** contains the ground truth annotation for 13 classes for NYUv2 training dataset while **test_labels_13** contains the ground truth for test dataset in NYUv2.

- The training dataset (795 RGB images) can be obtained from [nyu_train_rgb](http://www.doc.ic.ac.uk/~ahanda/nyu_train_rgb.tgz) while the test dataset (654 RGB images) can be obtained from [nyu_test_rgb](http://www.doc.ic.ac.uk/~ahanda/nyu_test_rgb.tgz).

## How do I obtain the DHA features?

Look for this in a corresponding [SUN RGB-D meta data repository](https://github.com/ankurhanda/sunrgbd-meta-data).

## How do I benchmark? 
[getAccuracyNYU.m](https://github.com/ankurhanda/SceneNetv1.0/blob/master/getAccuracyNYU.m) available in the [SceneNetv1.0](https://github.com/ankurhanda/SceneNetv1.0/) repository allows you to obtain the avereage global and class accuracies. 
