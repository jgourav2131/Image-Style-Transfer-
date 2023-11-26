The main goal of project is to combine two images and produce new image. The combination works in slightly different way i.e., we combine the style of one image with the content of other image. First we take the image from which we want to extract content usually called content image and take another image from which the style is to be extracted usually called style image.

Convolutional Neural Networks are a type of neural networks which are used widely in Image classification and recongnition. A CNN architecture called VGG19 has been used in this project. The starting layers in this architecture extract the basic features and shapes and later layers will extract more complex image patterns. So for the output image we will take the content from later layers of CNN. For extracting the style of image, we take the correlations between different layers using Gram Matrix

Initially, we take any random image as target(or taking the content image would be useful) and compute the Content loss and Style loss and decreasing these losses we would reach the perfect target image that has the style of one image and content of other image. For more learning checkout the links below.

CPU/GPU: The notebook has been ran on Kaggle GPU T4 x 20.

DATASET: I have used the 'best artwork of all time' dataset available on kaggle to extract the styles. This dataset consistes of many styles to choose from.

Languages or Frameworks Used
Python: language
NumPy: library for numerical calculations
Matplotlib: library for data visualisation
Pytorch: a deep learning framework by Facebook AI Research Team for building neural networks
torchvision: package consists of popular datasets, model architectures, and common image transformations for computer vision
