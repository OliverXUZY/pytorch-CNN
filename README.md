# pytorch-CNN
This is the final project of deep learing course STAT479 in 2019 fall intructed by Prof. Sebastian Raschka. The institute is UW-Madison.

## Main work
We propose a face-to-painting machine, which can identify a person and then produce a portrait of him/her automatically based on a given painting style.
  
On the first part of our project, we implement transfer learning of our own datasets to test the performance of different CNN architectures. We use several convolutional architectures and ResNet achieves the best result. Then, we use FaceNet methods to perform the face verification based on different CNN architectures: ResNet34, ResNet50, VGG16 and VGG19. The ResNet34 model gives the best test result on the LFW dataset, the test accuracy reaches 81.47\% after only 20 epochs, with AUC 0.90.We also introduce a neural style transfer method to generate the portraits in different painting styles. We choose the pre-trained VGG19 architecture to implement such method and the generated portraits are at least qualitatively comparable to common portrait paintings.

Our project can be used in many real world applications, like generating tourist attraction souvenir, building automatic painting system and so on. Our face-to-painting machine is easy to interpret, easy to train and it provides some insights into potential applications of deep learning methods. Based on our project, people can implement deep learning methods into wider fields and improve our methods to get better results.
