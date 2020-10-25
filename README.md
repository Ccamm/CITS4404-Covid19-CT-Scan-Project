# Repository for CITS4404 COVID 19 CT Scans

# How to Run 

## Generate COVID CT scan images using StyleGAN 2 (Cits4404_StyleGAN2_%2B_DiffAugment.ipynb)
1.   Run the Environment setup code block
2.   Run the evaluation code block. Generated pictures should be displayed in the output of the last code block


## Evaluate COVID CT scan images using InfoMax Gan and InfoMax Gan Transfer
(InfoMax Gan.ipynb and InfoMax Gan Transfer.ipynb)
1. Run all Setup code blocks before Training block
2. Run Evaluation code block to see Images generated 
  - Images generated will be an 8x8 grid of 128x128 images (64 images total in grid)
  - Images will be in $PWD/log/example/images
  - 2 images generated every 500 epochs: a fixed noise input image, and random noise input image
* Note that code to backup progress to google drive while training will not work unless google drive mounted on colab and paths are correct*

## Upscale Generated Images with ESRGAN (ESRGAN-UPSCALED.ipynb)
1. Run all code blocks to generate upscaled versions of sample images generated from StyleGan2 model above
* Can modify 'Specify Samples for Upscaling' code block to upscale with own images*
