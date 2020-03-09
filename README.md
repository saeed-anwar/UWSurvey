# Diving Deeper into Underwater Image Enhancement: A Survey
This repository is about the review of underwater image enhancement introduced in the following paper

[Saeed Anwar](https://saeed-anwar.github.io/), [Chongyi Li](https://li-chongyi.github.io/), "Diving Deeper into Underwater Image Enhancement: A Survey", [[arXiv]](https://arxiv.org/pdf/1907.07863.pdf) 


## Contents
1. [Introduction](#introduction)
2. [Overview](#overview)
3. [Datasets](#datasets)
4. [Results](#results)
5. [Ablation](#ablation)
6. [Citation](#citation)
7. [Acknowledgements](#acknowledgements)

## Introduction
The powerful representation capacity of deep learning has made it inevitable for the underwater image enhancement community to employ its potential. The exploration of deep underwater image enhancement networks is increasing over time, and hence, a comprehensive survey is the need of the hour. In this paper, our main aim is two-fold, 1): to provide a comprehensive and in-depth survey of the deep learning-based underwater image enhancement, which covers various perspectives ranging from algorithms to open issues, and 2): to conduct a qualitative and quantitative comparison of the deep algorithms on diverse datasets to serve as a benchmark, which has been barely explored before. 

We first introduce the underwater image formation models, which are the base of training data synthesis and design of deep networks, and also helpful for understanding the process of underwater image degradation. Then, we review deep underwater image enhancement algorithms, and a glimpse of some of the aspects of the current networks is presented, including architecture, parameters, training data, loss function, and training configurations. We also summarize the evaluation metrics and underwater image datasets. Following that, a systematically experimental comparison is carried out to analyze the robustness and effectiveness of deep algorithms. Meanwhile, we point out the shortcomings of current benchmark datasets and evaluation metrics. Finally, we discuss several unsolved open issues and suggest possible research directions. We hope that all efforts done in this paper might serve as a comprehensive reference for future research and call for the development of deep learning-based underwater image enhancement. 

## Overview
![Overview](/Figs/classification_nets.png)
An overview of the existing single-image super-resolution techniques.

![Networks](/Figs/UWESurveyFigs.png)
A glimpse of diverse range of network architectures used for single-image super-resolution using deep networks.

## Datasets
We compare the state-of-the-art algorithms on publicly available benchmark datasets which include Set5, Set14, BSD100, Urban100, DIV2K and
Manga109.
![Images](/Figs/RepresentativeImages.PNG)
Representative test images from six super-resolution datasets used for comparing and evaluating algorithms

## Results
### Quantitative Results
![PSNR_SSIM_2x](/Figs/2xTable.PNG)
![PSNR_SSIM_3x](/Figs/3xTable.PNG)
![PSNR_SSIM_4x](/Figs/4xTable.PNG)
Mean PSNR and SSIM for the SR methods evaluated on the benchmark datasets. The ’-’ indicates that the method is not suitable to handle the images of the corresponding dataset.

![PSNR_SSIM_8x](/Figs/8xTable.PNG)
The results for 8x Super-resolution.

### Visual Results

![Visual_PSNR_SSIM_BI](/Figs/Urban.PNG)
Super-resolution qualitative comparison for CNN-SR algorithms for 4x and 8x
![Visual_PSNR_SSIM_BI](/Figs/SR_GAN.PNG)
Visual comparison for GAN-SR algorithms for 4x

## Ablation
![PARAMETERS_TABLE](/Figs/parameters.PNG)

Parameters comparison of CNN-based SR algorithms. GRL stands for Global residual learning, LRL means Local residual learning, MST is
abbreviation of Multi-scale training.


<p align="center">
  <img width="500" src="https://github.com/saeed-anwar/SRsurvey/blob/master/Figs/mult_adds_comp.PNG">
</p>
Comparison of Multiplication-Addition operations in various SR networks. Note that FLOPs are roughly double the number of mult-adds.
Algorithmic runtime (during inference) is proportional to the multi-add operations.

<p align="center">
  <img width="500" src="https://github.com/saeed-anwar/SRsurvey/blob/master/Figs/params_comp.PNG">
</p>
Comparison of number of parameters in various SR architectures. The memory footprint and training time of the model is directly related to the number of tunable parameters.

## Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@article{anwar2019deep,
  title={A Deep Journey into Super-resolution: A survey},
  author={Anwar, Saeed and Khan, Salman and Barnes, Nick},
  journal={arXiv preprint arXiv:1904.07523},
  year={2019}
}

@article{anwar2019drln,
  title={Densely Residual Laplacian Super-Resolution},
  author={Anwar, Saeed and Barnes, Nick},
  journal={arXiv preprint arXiv:1906.12021},
  year={2019}
}

```
## Acknowledgements



