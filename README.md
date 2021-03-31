# Synthetic data generation on car parts
The project carried out as part of the Deep Learning course at Technical University of Denmark in collaboration
with Deloitte Denmark.

This project aims to create photo-realistic synthetic cars using generative adversarial networks(GANs).

Below is provided a short explanation on the jupyter files that this repository is consisted of.

The project flow is illustrated below.

![alt text](https://github.com/georgezefko/Synthetic-Data-Generation/blob/main/workflow.png?raw=true)

**-Syntehtic_data_generation**
This file containt the full written report on the project. 
You can read to understand the logic and scope behind the model. 
You will also get a better understanding about the process, limitations and future work of the project.

**-Read_data**
Code that includes data preprocessing such cropping and store them in correct folders

**-Deloitte data preprocessing**
The file contains the process followed in order to create the masks.

**-GAN_Deconvolution**
Refers to one of the two architectures tested and it is built as DCGAN. 

**-Gan_Interpolation**
Refers to the second architecture tested. Simple interpolation applied as upsampling instead of trasposed convolution
in order to obtain smoother images.

**-Pix2PixNVIDIA**
The [pix2pixHD](https://github.com/NVIDIA/pix2pixHD)  made by NVIDIA cloned in order to generate photorealistic images. 

**-FID_Pix2PixHD**
In order to calculate the FID score on the images generated from pix2pix we cloned the official implementation of [FID score for Pytorch](https://github.com/mseitzer/pytorch-fid)

# Improvement points and future work
 -  The data fed into the model should be balancedand exclude data with dissimilar semantic sizes.
 -  To overcome the limitations related to Stage-I process, we canuse an Auxiliary Classifier GAN . 
 -  For a better generation of photo-realistic images, we should give more data to pix2pixmodel during training.  
 -  The next step of the project will be to build a semantic segmentationmodel, to capture car parts on the synthetic images
