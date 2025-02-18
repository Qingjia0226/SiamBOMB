# <img src=".github/README/icon.png" width="22"> SiamBOMB

[![Commit](https://img.shields.io/github/last-commit/JackieZhai/SiamBOMB)](https://github.com/JackieZhai/SiamBOMB/commits/20210919)
![RepoSize](https://img.shields.io/github/repo-size/JackieZhai/SiamBOMB)
![CodeSize](https://img.shields.io/github/languages/code-size/JackieZhai/SiamBOMB)
[![PyPI](https://img.shields.io/pypi/v/SiamBOMB)](https://pypi.org/project/SiamBOMB)
[![Release](https://img.shields.io/github/v/release/JackieZhai/SiamBOMB?include_prereleases&sort=semver)](https://github.com/JackieZhai/SiamBOMB/releases)

This repo is the third preview version of SiamBOMB, which wil be updated until the end of 2021.\
Team of MiRA, Institute of Automation, CAS. <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/80x15.png" /></a> All rights reserved.
<p align="center"><img src=".github/README/affiliation.png" width="500"></p>

## Setup
### 1. Configure environments
TODO
```Shell
conda create -n SiamBOMB python=3.7
conda activate SiamBOMB
```
### 2. Install dependencies
TODO
```Shell
pip install --upgrade SiamBOMB
```
### 3. Equip models
Automatically, (with gdown from [Google Drive](https://drive.google.com))
```Shell
python -m SiamBOMB.downloader
```
Or manually,
* SiamMask_E pretrained model: [Google Drive](https://drive.google.com/u/0/uc?id=1VVpCAUJeysyRWdLdfW1IsT3AsQUQvwAU), 
[Baidu Pan](https://pan.baidu.com/s/1q64A2jPEWmdj264XrfvhBA) (jffj) \
into `pysot/experiments/siammaske_r50_l3/model.pth`
* KYS pretrained model: [Google Drive](https://drive.google.com/u/0/uc?id=13uOa9cpTyVf7hB3RkdjjN-hyEr4yJiSw), 
[Baidu Pan](https://pan.baidu.com/s/1el4NGj9LYn3lF_FNZv4Xig) (bf3u)\
into `pytracking/networks/kys.pth`
* LWL pretrained model: [Google Drive](https://drive.google.com/u/0/uc?id=18G1kAcLrTgO1Hgyj290mqPKsfVIkI9lw), 
[Baidu Pan](https://pan.baidu.com/s/1Xu79riptlOLorp0w3uQ3jw) (w244)\
into `pytracking/networks/lwl_boxinit.pth`
* KeepTrack pretrained model: [Google Drive](https://drive.google.com/u/0/uc?id=1zyadmon8codJDvOQlHAsBDPA_ouN4Zud), 
[Baidu Pan](https://pan.baidu.com/s/1W5Xxwrxl2Bge9nB1qWY2SQ) (g92v)\
into `pytracking/networks/keep_track.pth`\
and its base model: [Google Drive](https://drive.google.com/u/0/uc?id=1cRgzZ0MFFeE2PaZL3BWbYXu9Aq73f-TR), 
[Baidu Pan](https://pan.baidu.com/s/1w1-0kSRq1X2zu-k1mAqsoQ) (zylv)\
into `pytracking/networks/super_dimp_simple.pth`

You can download several of them on demand.

## Demonstration
TODO
```Shell
python -m SiamBOMB.launcher
```

## Citation
```
@inproceedings{SiamBOMB,
  title     = {SiamBOMB: A Real-time AI-based System for Home-cage Animal Tracking, Segmentation and Behavioral Analysis},
  author    = {Chen, Xi and Zhai, Hao and Liu, Danqian and Li, Weifu and Ding, Chaoyue and Xie, Qiwei and Han, Hua},
  booktitle = {Proceedings of the Twenty-Ninth International Joint Conference on
               Artificial Intelligence, {IJCAI-20}},
  publisher = {International Joint Conferences on Artificial Intelligence Organization},             
  pages     = {5300--5302},
  year      = {2020},
  month     = {7},
  doi       = {10.24963/ijcai.2020/776},
  url       = {https://doi.org/10.24963/ijcai.2020/776},
}
```

## References
```
@article{A_Common_Hub,
  title={A common hub for sleep and motor control in the substantia nigra},
  author={Liu, Danqian and Li, Weifu and Ma, Chenyan and Zheng, Weitong and Yao, Yuanyuan and Tso, Chak Foon and Zhong, Peng and Chen, Xi and Song, Jun Ho and Choi, Woochul and others},
  journal={Science},
  volume={367},
  number={6476},
  pages={440--445},
  year={2020},
  publisher={American Association for the Advancement of Science}
}
```
