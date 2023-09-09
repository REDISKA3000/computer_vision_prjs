# Computer Vision projects

Here I present the results of my experinece and exploration in CV. There are 5 projects that consider distinct tasks from basic classification to stylization using advanced DL architectures.

### Simpsons classification. 
This project is devoted to the image classification task. For the training i used the dataset with images of charachters from "The Simpsons". The main difficulty of the dataset is the imbalance of classes, as some characters occured more often in the series than others. To tackle the issue I used a variety of data augmentation methods to generate more images of classes with smaller sammples. As for the model, after efficient data prepocessing it was enough to construct standard CNN and train it, so that to achieve **F1_score > 0.97**.
### Autoencoders
The folder contains 2 notebooks: denoising and image reconstruction (basic generation). In the first notebook I used 3 types of autoencoders: basic autoencoder (AE), variational AE (VAE) and conditional VAE (CVAE), and trained them on the dataset with face images (more detailed explanation of architectures is in the notebook). To imrove the result on the validset, I implemeted **KL-divergency loss-function** and used it for training. In the second notebook I used the same dataset with faces and added gaussain noise to each image. To denoise these images I applied AE model and obtained well result. 
### ADDI project
Segmentation is a common problem in CV, that has already found many applications in real life. Cancer segmentation is such problem, which aims to segment skin images infected by cancer into 2 group: infected part of skin and uninfected. To solve this problem I contsrusted 3 distinct models SegNet, UNet and UNet2 (detailed description is in the notebook, UNet2 is modifies UNet).
Also I implemented several distinct loss-functions: **Dice, Focal, Tversky, Lovasz**, and compared model trained with them. In the end of the notebook one can see plotted losses.
### GAN generation

