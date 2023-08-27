# Deep Generative Denoising: 
***An exploration of re-synthesis as an alternative to subtractive methods of denoising an acoustic guitar signal***

## Is generative denoising an oxymoron?
While generative denoising may sound a little bit like "additive subtraction", the basic idea behind this approach to audio enhancement is that the model is estimating the clean audio signal directly rather than estimating the noise that needs to be subtracted. In other words, **rather than learning what noise sounds like, the model learns what an acoustic guitar sounds like.** 

## Why generative denoising?
While subtractive methods like binary and ratio mask estimation may be more efficient in the short term, the two advantages that pushed me toward exploring generative denoising were the possibilities of **1) Upscaling Audio Quality** and **2) Personalization**. 

#### Upscaling Audio Quality
Without getting too in the weeds, the complex interraction of overlapping sound waves makes a noisy signal more (or less) than a simple sum of its parts. This means that a simple subtraction of the noisy elements of the signal can never recover what a recording would have sounded like if the noise had not been present. By training a model to synthesize a clean signal based on a compressed version of a noisy signal, it is possible to not only retrieve something close to a clean version 
