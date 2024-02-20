### This repo explain how DDPM and Stable Diffusion work

### [Denoising Diffusion Probabilistic Models (DDPM)](./DDPM.ipynb) 

By using special technic in Diffusion Process and Markov Chain, DDPM can reverse the process, therefore generate image from a random noise. It use UNET as its backbone, trying to minimize the loss for the reconstruction.

### [Stable Diffusion](./Stable_Diffusion.ipynb)

With DDPM, Latent Diffusion Model (LDM) and CLIP, researchers are able to create State-Of-The-Art Generative Model for image. 

It recieves text or/and image as an input (Img2Img, Text2Img). The image will passing through an VAE Encoder blocks and the text will go through CLIP to the latent space. Then the DDPM does its magic in latent space, and the Decoder Block of VAE will generate new image from that output