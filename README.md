# pytorch-CNN
This is the final project of deep learing course STAT479 in 2019 fall intructed by Prof. Sebastian Raschka. The institute is UW-Madison.

## Main work
We propose a face-to-painting machine, which can identify a person and then produce a portrait of him/her automatically based on a given painting style.
  
On the first part of our project, we implement transfer learning of our own datasets to test the performance of different CNN architectures. We use several convolutional architectures and ResNet achieves the best result. Then, we use FaceNet methods to perform the face verification based on different CNN architectures: ResNet34, ResNet50, VGG16 and VGG19. The ResNet34 model gives the best test result on the LFW dataset, the test accuracy reaches 81.47\% after only 20 epochs, with AUC 0.90.We also introduce a neural style transfer method to generate the portraits in different painting styles. We choose the pre-trained VGG19 architecture to implement such method and the generated portraits are at least qualitatively comparable to common portrait paintings.

Our project can be used in many real world applications, like generating tourist attraction souvenir, building automatic painting system and so on. Our face-to-painting machine is easy to interpret, easy to train and it provides some insights into potential applications of deep learning methods. Based on our project, people can implement deep learning methods into wider fields and improve our methods to get better results.

keyword: Deep CNN architecture, Transfer learning, Triplet loss, Neural style transfer 

## Data
- **Transfer Learning and Neural Style Transfer** We use [icrawler 0.6.2 package](https://icrawler.readthedocs.io/en/latest/index.html) to scrape images from Google Image Search by ourselves. We perform some pre-rpcessing to the images and split them into train and test samples. This database contains images of 15 celebrities like Gal Gadot, Robert Downey Jr etc. There are around 7500 images in total. This dataset is mainly used in the transfer learning part and the neural style transfer part.

- **FaceNet system** For the face verification using FaceNet, we use [Labeled Face in the Wild (LFW)](http://vis-www.cs.umass.edu/lfw/) dataset. It is a database of face photographs designed for studying the problem of unconstrained face recognition. The data set contains more than 13,000 images of faces collected from the web, for nearly 6000 people. Among of them, around 1700 people have two or more images


## Contributions
Zhuoyan Xu (zxu444@wisc.edu) implements the transfer learning and FaceNet system for the face verification. He also scrapes the data on Google image search for the transfer learning, and implements the data augmentation and other pre-processing work. He writes the related work, proposed method, experiment, result and conclusion part of the project. 

Lingfeng Zhu (lzhu88@wisc.edu) implements the neural style transfer and transfer learning,
he writes the abstract part, result and conclusion part and related works part and comes up with the proposed method part in our project report. 

Cercily Liu (qliu273@wisc.edu) helped with the data collection and data pre-processing part. She implements the data augmentation and transfer learning. She also  write the introduction and motivation part for the project report.

## Acknowleagement
We are glad to acknowledge Prof. Sebastian Raschka, without whose instruction we will not be able to establish and finish this project, let alone entering this interesting world of deep learning. Last but not least, we would like to acknowledge Overleaf and Github, they make cooperation more easier than ever.

## References
- [Course home page](https://github.com/Dumplings-whu/stat479-deep-learning-ss19)
- [faceNet pytorch implementation](https://github.com/tbmoon/facenet)
- paper,data references of our project report

