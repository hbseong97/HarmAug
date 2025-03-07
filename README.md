# HarmAug: Effective Data Augmentation for Knowledge Distillation of Safety Guard Models
This repository contains code for reproducing HarmAug introduced in

**HarmAug: Effective Data Augmentation for Knowledge Distillation of Safety Guard Models**

Seanie Lee*, Haebin Seong*, Dong Bok Lee, Minki Kang, Xiaoyin Chen, Dominik Wagner, Yoshua Bengio, Juho Lee, Sung Ju Hwang (*: Equal contribution)

[[arXiv link]](https://arxiv.org/abs/2410.01524)  
[[Model link]](https://huggingface.co/hbseong/HarmAug-Guard)  
[[Dataset link]](https://huggingface.co/datasets/hbseong/HarmAug_generated_dataset)


![concept_figure](https://github.com/user-attachments/assets/3e61f7c6-e0c2-4107-bb4e-9b4d2c7ba961)

![overall_comparison_broken](https://github.com/user-attachments/assets/03cc0fa5-e9dc-4d78-a5b8-a2c122672fea)



## Reproduction Steps

First, we recommend to create a conda environment with python 3.10.
```
conda create -n harmaug python=3.10
conda activate harmaug
```


After that, install the requirements.
```
pip install -r requirements.txt
```


Then, download necessary files from [Google Drive](https://drive.google.com/drive/folders/1oLUMPauXYtEBP7rvbULXL4hHp9Ck_yqg?usp=drive_link) and put them into their appropriate folders.
```
mv kd_dataset@harmaug.json ./data
```


Finally, you can start the knowledge distillation process.
```
bash script/kd.sh
```

## Reference
To cite our paper, please use this BibTex
```bibtex
@inproceedings{
lee2025harmaug,
title={HarmAug: Effective Data Augmentation for Knowledge Distillation of Safety Guard Models},
author={Seanie Lee and Haebin Seong and Dong Bok Lee and Minki Kang and Xiaoyin Chen and Dominik Wagner and Yoshua Bengio and Juho Lee and Sung Ju Hwang},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://openreview.net/forum?id=y3zswp3gek}
}
