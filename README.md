# Paper Collection on Diffusion Models 

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/hee9joon/Awesome-Diffusion-Models) 


This repository contains a collection of papers on ***Diffusion Models***.

It's a simple way for me to keep track of the papers I've read and the ones I want to read.  Every paper will be summarized in a few sentences. Read papers are marked with a :zap:

Feel free to browse through the papers and summaries. Happy reading!




## Contributions

If you'd like to contribute to this repository by adding papers or improving summaries, please submit a pull request. Your contributions are greatly appreciated!

To add a new paper to the repository, follow these steps:

- Summarize the paper in a few sentences.
- Add the paper title, authors, and a link to the paper.


## Contents
- [Resources](#resources)
  - [Introductory Posts](#introductory-posts)
  - [Introductory Papers](#introductory-papers)
  - [Introductory Videos](#introductory-videos)

- [Papers](#papers)
  - [Must-Read](#must-read)
  - [Personalization](#personalization)


# Resources
## Introductory Posts

**What are Diffusion Models?** :zap: \
*Lilian Weng* \
[[Website](https://lilianweng.github.io/lil-log/2021/07/11/diffusion-models.html)] \
Jul 2021


**DiffusionFastForward: 01-Diffusion-Theory** :zap: \
*Mikolaj Czerkawski (@mikonvergence)* \
[[Website](https://github.com/mikonvergence/DiffusionFastForward/blob/master/notes/01-Diffusion-Theory.md)] \
Feb 2023


**Diffusion Models as a kind of VAE**  :zap: \
*Angus Turner* \
[[Website](https://angusturner.github.io/generative_models/2021/06/29/diffusion-probabilistic-models-I.html)] \
Jun 2021


**Generative Modeling by Estimating Gradients of the Data Distribution** :zap: \
*Yang Song* \
[[Website](https://yang-song.github.io/blog/2021/score/)] \
May 2021

## Introductory Papers

**Understanding Diffusion Models: A Unified Perspective** :zap: \
*Calvin Luo* \
arXiv 2022. [[Paper](https://arxiv.org/abs/2208.11970)] \
A good intro to Diffusion Models from VAE to DDPM with the math from scratch.

**How to Train Your Energy-Based Models** \
*Yang Song, Diederik P. Kingma* \
arXiv 2022. [[Paper](https://arxiv.org/abs/2101.03288)] \
A good intro focused
on maximum likelihood estimation with MCMC sampling, Score Matching, and Noise
Contrastive Estimation. 


**Diffusion Models: A Comprehensive Survey of Methods and Applications** \
*Ling Yang, Zhilong Zhang, Shenda Hong, Wentao Zhang, Bin Cui* \
arXiv 2022. [[Paper](https://arxiv.org/abs/2209.00796)]  [[Collection](https://github.com/YangLing0818/Diffusion-Models-Papers-Survey-Taxonomy)]\
Survey.


## Introductory Videos

**Diffusion Models | Paper Explanation | Math Explained** \
*Outlier* \
[[Video](https://www.youtube.com/watch?v=HoKDTa5jHvg)] \
Exlains the derivation of the DDPM loss well.

**What are Diffusion Models?** \
*Ari Seff* \
[[Video](https://www.youtube.com/watch?v=fbLgFrlTnGU&list=LL&index=2)] \
Nice conection to VAE.


**DiffusionFastForward** \
*Mikolaj Czerkawski (@mikonvergence)* \
[[Video](https://www.youtube.com/playlist?list=PL5RHjmn-MVHDMcqx-SI53mB7sFOqPK6gN)] \
A series of videos on Diffusion from DDPM to High-Resolution.




## Must-Read

**Deep Unsupervised Learning using Nonequilibrium Thermodynamics** :zap: \
*Jascha Sohl-Dickstein, Eric A. Weiss, Niru Maheswaranathan, Surya Ganguli* \
ICML 2015. [[Paper](https://arxiv.org/abs/1503.03585)] [[Github](https://github.com/Sohl-Dickstein/Diffusion-Probabilistic-Models)] \
The first paper. Proposes a method to recover data through reverse diffusion process. Worth reading in order to understand the connection with statistical physics.

**Denoising Diffusion Probabilistic Models** :zap: \
*Jonathan Ho, Ajay Jain, Pieter Abbeel* \
NeurIPS 2020. [[Paper](https://arxiv.org/abs/2006.11239)] [[Github](https://github.com/hojonathanho/diffusion)] [[Github2](https://github.com/pesser/pytorch_diffusion)] \
The comeback. Proposed a method of sampling $x_t$ directly from $x_0$, and simplified the diffusion loss. 

**Improved Denoising Diffusion Probabilistic Models** :zap:\
*Alex Nichol<sup>1</sup>, Prafulla Dhariwal<sup>1</sup>* \
ICLR 2021. [[Paper](https://arxiv.org/abs/2102.09672)] [[Github](https://github.com/openai/improved-diffusion)] \
Main contribution of this paper is a method to learning the variance in the backward process as an interpolation between $\beta_t$ and $\bar{\beta}_t$.

**Variational Diffusion Models** :zap:\
*Diederik P. Kingma, Tim Salimans, Ben Poole, Jonathan Ho* \
NeurIPS 2021. [[Paper](https://arxiv.org/abs/2107.00630)] [[Github](https://github.com/revsic/jax-variational-diffwave)] \
1 Jul 2021 \
A method to learn the noise schedule by modeling the $SNR=\frac{\mu^2}{\sigma^2}$.


**Diffusion Models Beat GANs on Image Synthesis** :zap:\
*Prafulla Dhariwal<sup>1</sup>, Alex Nichol<sup>1</sup>* \
arXiv 2021. [[Paper](https://arxiv.org/abs/2105.05233)] [[Github](https://github.com/openai/guided-diffusion)] \
Proposed Classifier Guidance and other improvments on architecture.

**Denoising Diffusion Implicit Models** :zap: \
*Jiaming Song, Chenlin Meng, Stefano Ermon* \
ICLR 2021. [[Paper](https://arxiv.org/abs/2010.02502)] [[Github](https://github.com/ermongroup/ddim)] \
Brakes the Markov chain constraint and makes the reverse process deterministic. This allows to skip steps and make sampling a lot faster. A bit mathematically complex but is a must read.

**Generative Modeling by Estimating Gradients of the Data Distribution** :zap: \
*Yang Song, Stefano Ermon* \
NeurIPS 2019. [[Paper](https://arxiv.org/abs/1907.05600)] [[Project](https://yang-song.github.io/blog/2021/score/)] [[Github](https://github.com/ermongroup/ncsn)] \
First paper of Score-Based Models.

**Score-Based Generative Modeling through Stochastic Differential Equations** \
*Yang Song, Jascha Sohl-Dickstein, Diederik P. Kingma, Abhishek Kumar, Stefano Ermon, Ben Poole* \
ICLR 2021 (Oral). [[Paper](https://arxiv.org/abs/2011.13456)] [[Github](https://github.com/yang-song/score_sde)] \
A paper that combines DDPM and Score-Based models under an SDE framework.



**Elucidating the Design Space of Diffusion-Based Generative Models** \
*Tero Karras, Miika Aittala, Timo Aila, Samuli Laine* \
arXiv 2022. [[Paper](https://arxiv.org/abs/2206.00364)] \
Implementation improvements

**Classifier-Free Diffusion Guidance** \
*Jonathan Ho, Tim Salimans* \
NeurIPS Workshop 2021. [[Paper](https://arxiv.org/abs/2207.12598)] \
Instead of providing guidance from an external classifier (Classifier Guidance), conditions are plugged into the UNet.

**High-Resolution Image Synthesis with Latent Diffusion Models** :zap:\
*Robin Rombach, Andreas Blattmann, Dominik Lorenz, Patrick Esser, Björn Ommer* \
CVPR 2022. [[Paper](https://arxiv.org/abs/2112.10752)] \
Perform the diffusion process on a latent space instead of the image space.


## Personalization
**An Image is Worth One Word: Personalizing Text-to-Image Generation using Textual Inversion** :zap:\
*Rinon Gal, Yuval Alaluf, Yuval Atzmon, Or Patashnik, Amit H. Bermano, Gal Chechik, Daniel Cohen-Or* \
ICLR 2023 Spotlight [[Paper](https://arxiv.org/abs/2208.01618)] [[Code](https://github.com/rinongal/textual_inversion)] [[Project Page](https://textual-inversion.github.io/)] \
Learn to generate and manipulate specific concepts by training word embedding.


**DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation** :zap:\
*Nataniel Ruiz, Yuanzhen Li, Varun Jampani, Yael Pritch, Michael Rubinstein, Kfir Aberman* \
CVPR 2023 [[Paper](https://arxiv.org/abs/2208.12242)] [[Code](https://github.com/google/dreambooth)] [[Project Page](https://dreambooth.github.io/)] \
Learn to generate and manipulate specific concepts by finetuning the hole model with an additional prior preservation loss.
