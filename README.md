# TransWeather

 <a href="https://arxiv.org/abs/2111.14813"> </a> 

Official Code for the paper [TransWeather: Transformer-based Restoration of Images Degraded by Adverse Weather Conditions](https://arxiv.org/abs/2111.14813), CVPR 2022

[Paper](https://arxiv.org/abs/2111.14813) | [Website](https://jeya-maria-jose.github.io/transweather-web/)

### About this repo:

This repo hosts the implentation code for the paper "TransWeather". We also provide code for a strong transformer baseline for weather removal tasks.

## Introduction

Removing adverse weather conditions like rain, fog, and snow from images is an important problem in many applications. Most methods proposed in the literature have been designed to deal with just removing one type of degradation. Recently, a CNN-based method  using neural architecture search (All-in-One) was proposed  to remove all the weather conditions at once. However, it has a large number of parameters as it uses multiple encoders to cater to each weather removal task and still has scope for improvement in its performance. In this work, we focus on developing an efficient solution for the all adverse weather removal problem. To this end, we propose TransWeather, a transformer-based end-to-end model with just a single encoder and a decoder that can restore an image degraded by any weather condition. Specifically, we utilize a novel transformer encoder using intra-patch transformer blocks to enhance attention inside the patches to effectively remove smaller weather degradations. We also introduce a transformer decoder with learnable weather type embeddings to adjust to the weather degradation at hand. TransWeather achieves significant improvements across multiple test datasets over both All-in-One network as well as methods fine-tuned for specific tasks. 

<p align="center">
  <img src="imgs/Transweather.png" width="800"/>
</p>

