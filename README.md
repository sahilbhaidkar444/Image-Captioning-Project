# What is Image Captioning ?
- Image Captioning is the process of generating a textual description for given images. <br>It has been a very important and fundamental task in the Deep Learning domain.

# What is the use of Image Captioning Project ?
There are various examples where this project can be useful:
- Aid to the blind
- Self driving cars
- Google Image Search
- CCTV Cameras

# Dataset Used in this project 
There are various open source datasets available over internet like :
- #### Flicker8k Dataset</b>
- Flicker 30k dataset
- MS Coco with 180k images

# Pre-processing the data :
I need to pre-process the image and caption data before the prediction of our model :
- For image data we need to convert the image data into fixed size i.e (24 X 24 pixel in my case).
- Next step is to pre-process our text data so that our model can understand the vocabulary to describe the images. So for that purpose I did some NLP on top of it before that I removed unwanted data from the text like stopwords , numbers and punctuation marks.
- And add the start and end sequence to each caption. For understanding the start and end of the caption.
- After preprocessing is done we need to convert the text data into machine understandable language.

# About Image Model :
- For image model I used Vgg16 model of 16 layer deep pretrained model
- Which is the process of transfer learning.
- VGG 16 was proposed by Karen Simonyan and Andrew Zisserman of the Visual Geometry Group Lab of Oxford University in 2014 in the paper “VERY DEEP CONVOLUTIONAL NETWORKS FOR LARGE-SCALE IMAGE RECOGNITION”.
- This model achieves 92.7% top-5 test accuracy on the ImageNet dataset which contains 14 million images belonging to 1000 classes.

# About Captioning model :
- Captioning model relies on LSTM . Captioning is all about merging two things.
- LSTM model is a sequential model which works with any kind of sequential data such as sequence of words.
- So by merging of two models you will get a model that can find the patterns and images that can then generate captions related to the images.

# Model Performance :
![image](https://user-images.githubusercontent.com/44014705/180954001-7ecddd0e-1c6d-4593-a711-e95b52a9dc62.png)

# Output :
![image](https://user-images.githubusercontent.com/44014705/180954261-93de12c9-5f45-48d3-ade0-a42a60b72722.png)
