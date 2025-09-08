# All-Day Multi-Camera Multi-Target Tracking

[Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Fan_All-Day_Multi-Camera_Multi-Target_Tracking_CVPR_2025_paper.pdf)

This repository is an official implementation of [AMCMT](https://openaccess.thecvf.com/content/CVPR2025/papers/Fan_All-Day_Multi-Camera_Multi-Target_Tracking_CVPR_2025_paper.pdf) model and M3Track dataset.


## Abstract


![Overview](img/model.png)

 In this paper, we propose ADMCMT, which is the first MCMT tracking model for low-light environments. Specifically, we propose an All-Day Mamba Fusion (ADMF) module to adaptively fuse information from different modalities. Within ADMF, the Lighting Guidance Model (LGM) extracts lighting relevant information to guide the fusion process. Furthermore, the Nearby Target Collection (NTC) strategy is designed to enhance tracking accuracy by leveraging information derived from surrounding objects of target. Experiments conducted on M3Track demonstrate that ADMCMT exhibits strong generalization across different lighting conditions. We also constructed the first Multi-modality (RGBT) Multi-camera Multi-target tracking dataset named M3Track. In addition to incorporating multiple modalities, it also significantly surpasses existing multi-camera multi-object datasets in both scale and diversity.

## Main Results

### M3Track

| Method   | MOTA↑ | HOTA↑ | IDF1↑ | DetA↑ | MOTP↑ | MDA↑   | CVIDF1↑ | CVMA↑ |
|----------|-------|-------|-------|-------|-------|--------|---------|-------|
| OSNet    | 68.03 | 50.33 | 61.60 | 55.71 | 75.78 | 0.2756 | 48.50   | 28.60 |
| CrossMOT | 65.30 | 44.84 | 59.91 | 48.62 | 75.54 | 0.2019 | 51.21   | 38.51 |
| CT       | 68.21 | 50.38 | 61.17 | 55.89 | 75.80 | 0.4340 | 53.65   | 44.71 |
| MvMHAT   | 66.39 | 48.60 | 58.96 | 54.99 | 75.77 | 0.2178 | 46.64   | 26.72 |
| AGW      | 67.62 | 50.44 | 62.02 | 55.54 | 71.54 | 0.4235 | 54.81   | 45.02 |
| Ours     | **70.94** | **56.62** | **71.47** | **57.89** | **77.21** | **0.6169** | **68.77** | **61.81** |



## Plan for Open-Sourcing

Since our work is based on the unpublished [GMT](https://arxiv.org/pdf/2407.01007), we are unable to release the code now. We will release the code as soon as GMT is published.

## M3Track dataset

### Introduction
![Example](img/dataset.jpg)
![Compare](img/dataset_tj2.jpg)
M3Track is the first multi-camera multi-target tracking dataset that includes the infrared modality. Compared with existing datasets, M3Track is larger in scale and contains data captured under different weather conditions, at various times of the day, with varying target densities, and across diverse scenes, offering rich diversity.


### Download link
For commercial use, please contact the authors for authorization.

OneDrive: [Link](https://1drv.ms/f/c/140da35392af8a02/EqjdrWgGcjFGvk2Pc61fBzoBmSqWl1L6EVrb6kchVYqzcQ?e=AKWaBe)

BaiduNetdisk: [link](https://pan.baidu.com/s/1g0qaoyGUTZWJl3yNtR4rzw)  &emsp;&emsp;  Code: mcmt

## Citation
If you find this project useful for your research, please use the following BibTeX entry.

    @InProceedings{Fan_2025_CVPR,
        author    = {Fan, Huijie and Qiao, Yu and Zhen, Yihao and Zhao, Tinghui and Fan, Baojie and Wang, Qiang},
        title     = {All-Day Multi-Camera Multi-Target Tracking},
        booktitle = {Proceedings of the Computer Vision and Pattern Recognition Conference (CVPR)},
        month     = {June},
        year      = {2025},
        pages     = {16892-16901}
    }
