# Diving Deeper into Underwater Image Enhancement: A Survey
This repository is about the review of underwater image enhancement introduced in the following paper

[Saeed Anwar](https://saeed-anwar.github.io/), [Chongyi Li](https://li-chongyi.github.io/), "Diving Deeper into Underwater Image Enhancement: A Survey", accepted in Signal Processing: Image Communication, 2020, [[PDF]](https://arxiv.org/pdf/1907.07863.pdf) 


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
![Overview](/Fig/classification_nets.png)
An overview of the existing Underwater Image Enhancement and Restoration techniques.

![Networks](/Fig/UWESurveyFigs.png)
A glimpse of diverse range of network architectures used for Underwater image enhancement using deep networks.

## Datasets
We compare the state-of-the-art algorithms on publicly available benchmark datasets which include Haze-line, ULFID, and UIEBD.

![Images](/Fig/DatasetSampleImages.PNG)
Three sample images from Haze-line, ULFID, and UIEBD  datasets to show the diversity of the underwater images.

## Results
### Quantitative Results
![Six_evaluation_factors](/Fig/TableEvaluation.PNG)
Mean PSNR, MSE, SSIM, PCQI, UCIQE and UIQM evaluation metrics for the  methods evaluated on the benchmark dataset. The best results are highlighted with red color while the blue color represents the second best.

### Visual Results

![Visual_Greenish_comparison](/Fig/Greenish1.PNG)
![Visual_Greenish_comparison](/Fig/Greenish2.PNG)

Visual comparison of greenish images: Comparisons of different methods on the greenish underwater samples from
UIEBD. Here, UWCNN-type-I represents the model trained by synthetic type-I training data.

![Visual_Greenish_comparison](/Fig/bluish1.PNG)
![Visual_Greenish_comparison](/Fig/bluish2.PNG)

Qualitative comparisons on bluish images: The results of various CNN-based and GAN-based methods on the sample
underwater images from UIEBD.


![Visual_Greenish_comparison](/Fig/HighBackScatter.PNG)
![Visual_Greenish_comparison](/Fig/LowBackScatter.PNG)

The low and high backscatter images: The challenging images to remove the backscatter. The images are selected
from UIEBD dataset. The top image shows the low backscatter, while the bottom image illustrates the high backscatter.


![Visual_Greenish_comparison](/Fig/Hazeline1.PNG)
![Visual_Greenish_comparison](/Fig/Hazeline2.PNG)

Visual comparisons on Haze-line: The Haze-line dataset provides an accurate distance based on the stereo. To be
fair to the authors of Haze-line, we have also included the results of the best performer (i.e., Haze-line, a conventional
method) on this dataset.


![Visual_Greenish_comparison](/Fig/ULFID1.PNG)
![Visual_Greenish_comparison](/Fig/ULFID2.PNG)

Images from ULFID: A challenging dataset where all the methods fail to provide clean results.

## Ablation
![PARAMETERS_TABLE](/Fig/TableParameters.PNG)

Network Specifics: Essential parameters of underwater image enhancement and restoration networks. The losses i.e., lgan, lc , lW , lnui, lr and lg represents adversarial, consistency, Wasserstein, nuisance, relativistic and gradient losses, respectively. The “-” means information is not available.


## Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@article{Anwar2019UWESurvey,
  author = {Anwar, Saeed and Li, Chongyi},
    title = {Diving Deeper into Underwater image enhancement: A survey},
  journal = {ArXiv e-prints},
archivePrefix = "arXiv",
   eprint = {1907.07863},
 primaryClass = "cs.CV",
     year = 2019,
}

@article{Anwar2019UWE,
  title={Underwater Scene Prior Inspired Deep Underwater Image and Video Enhancement},
  author={Li, Chongyi and Anwar, Saeed},
  journal={Pattern Recognition},
  pages={107038},
  year={2019},
  publisher={Elsevier}
}

```
## Acknowledgements



