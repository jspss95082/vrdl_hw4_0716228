---
title: 'VRDL HW4 0716228'
disqus: hackmd
---

VRDL HW4 0716228
===





## Table of Contents

[TOC]

## How to generate answer.json?

1.  git clone this project
2.  Download train dataset  from [here](https://drive.google.com/file/d/1oTJMFz8qf9ZoUbURdt94aKjI3BF4PZiz/view?usp=sharing) 
and unzip it put it into `vrdl/hw4/0716228`
3.  Download pretrained model and data for testing from [here](https://drive.google.com/file/d/14-tE6WIW98qGODu7NcxxtKRFeyuUTuxa/view?usp=sharing) and unzip it into `vrdl_hw4_0716228\KAIR-master\testsets`
4.  `cd KAIR-master`
5.  `pip install -r requirements.txt`
6.  `python main_test_swinir.py --task classical_sr --scale 3 --model_path testsets/40000_G.pth --folder_lq testsets/testing_lr_images/testing_lr_images --folder_gt testsets/answerx3 --training_patch_size 48`
7.  output images is in `vrdl_hw4_0716228\KAIR-master\results\swinir_classical_sr_x3`

## How to train the model
1.  git clone this project
2.  Download train dataset  from [here](https://drive.google.com/file/d/1oTJMFz8qf9ZoUbURdt94aKjI3BF4PZiz/view?usp=sharing) 
and unzip it put it into `vrdl/hw4/0716228`
3. run all cell in `prepare_training.ipynb`
3.  Download validating from [here](https://drive.google.com/file/d/14-tE6WIW98qGODu7NcxxtKRFeyuUTuxa/view?usp=sharing) and unzip it into `vrdl_hw4_0716228\KAIR-master\testsets`
4.  `cd KAIR-master`
5.  `pip install -r requirements.txt`
6.  `python main_train_psnr.py --opt options/swinir/train_swinir_sr_classical.json`
7.  model will be put into `vrdl_hw4_0716228\KAIR-master\superresolution\swinir_sr\models`



## Pretrained model link
[link](https://drive.google.com/file/d/14-tE6WIW98qGODu7NcxxtKRFeyuUTuxa/view?usp=sharing)



#### `prepare_training.ipynb` was wirtten by me, so others don't follow PEP8

###### tags: `VRDL` `SwinIR`