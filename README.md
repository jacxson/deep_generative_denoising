# Deep Generative Denoising: 
***An exploration of re-synthesis as an alternative to subtractive methods of denoising an acoustic guitar signal***

## Is generative denoising an oxymoron?
While generative denoising may sound a little bit like "additive subtraction", the basic idea behind this approach to audio enhancement is that the model is estimating the clean audio signal directly rather than estimating the noise that needs to be subtracted. In other words, **rather than learning what noise sounds like, the model learns what an acoustic guitar sounds like.** 

## Why generative denoising?
While subtractive methods like binary and ratio mask estimation may be more efficient in the short term, the two advantages that pushed me toward exploring generative denoising were the possibilities of **1) Upscaling Audio Quality** and **2) Personalization**
