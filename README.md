# Synthetic data generation on car parts
The project carried out as part of the Deep Learning course at Technical University of Denmark in collaboration
with Deloitte Denmark.

This project aims to create photo-realistic synthetic cars using generative adversarial networks(GANs).

Below is provided a short explanation on the jupyter files that this repository is consisted of.

The project flow is illustrated below.

![alt text](https://github.com/georgezefko/Synthetic-Data-Generation/blob/main/workflow.png?raw=true)

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

