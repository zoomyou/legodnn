# Unified Perceptual Parsing for Scene Understanding

## Introduction

<!-- [ALGORITHM] -->

<a href="https://github.com/CSAILVision/unifiedparsing">Official Repo</a>

<a href="https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13">Code Snippet</a>

<details>
<summary align="right"><a href="https://arxiv.org/pdf/1807.10221.pdf">UPerNet (ECCV'2018)</a></summary>

```latex
@inproceedings{xiao2018unified,
  title={Unified perceptual parsing for scene understanding},
  author={Xiao, Tete and Liu, Yingcheng and Zhou, Bolei and Jiang, Yuning and Sun, Jian},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={418--434},
  year={2018}
}
```

</details>

## Results and models

### Cityscapes

| Method  | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                     | download                                                                                                                                                                                                                                                                                                                                               |
| ------- | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | -------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| UPerNet | R-50     | 512x1024  |   40000 | 6.4      | 4.25           | 77.10 |         78.37 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x1024_40k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_40k_cityscapes/upernet_r50_512x1024_40k_cityscapes_20200605_094827-aa54cb54.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_40k_cityscapes/upernet_r50_512x1024_40k_cityscapes_20200605_094827.log.json)     |
| UPerNet | R-101    | 512x1024  |   40000 | 7.4      | 3.79           | 78.69 |         80.11 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x1024_40k_cityscapes.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_40k_cityscapes/upernet_r101_512x1024_40k_cityscapes_20200605_094933-ebce3b10.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_40k_cityscapes/upernet_r101_512x1024_40k_cityscapes_20200605_094933.log.json) |
| UPerNet | R-50     | 769x769   |   40000 | 7.2      | 1.76           | 77.98 |         79.70 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_769x769_40k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_40k_cityscapes/upernet_r50_769x769_40k_cityscapes_20200530_033048-92d21539.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_40k_cityscapes/upernet_r50_769x769_40k_cityscapes_20200530_033048.log.json)         |
| UPerNet | R-101    | 769x769   |   40000 | 8.4      | 1.56           | 79.03 |         80.77 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_769x769_40k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_40k_cityscapes/upernet_r101_769x769_40k_cityscapes_20200530_040819-83c95d01.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_40k_cityscapes/upernet_r101_769x769_40k_cityscapes_20200530_040819.log.json)     |
| UPerNet | R-50     | 512x1024  |   80000 | -        | -              | 78.19 |         79.19 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x1024_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_80k_cityscapes/upernet_r50_512x1024_80k_cityscapes_20200607_052207-848beca8.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_80k_cityscapes/upernet_r50_512x1024_80k_cityscapes_20200607_052207.log.json)     |
| UPerNet | R-101    | 512x1024  |   80000 | -        | -              | 79.40 |         80.46 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x1024_80k_cityscapes.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_80k_cityscapes/upernet_r101_512x1024_80k_cityscapes_20200607_002403-f05f2345.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_80k_cityscapes/upernet_r101_512x1024_80k_cityscapes_20200607_002403.log.json) |
| UPerNet | R-50     | 769x769   |   80000 | -        | -              | 79.39 |         80.92 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_769x769_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_80k_cityscapes/upernet_r50_769x769_80k_cityscapes_20200607_005107-82ae7d15.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_80k_cityscapes/upernet_r50_769x769_80k_cityscapes_20200607_005107.log.json)         |
| UPerNet | R-101    | 769x769   |   80000 | -        | -              | 80.10 |         81.49 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_769x769_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_80k_cityscapes/upernet_r101_769x769_80k_cityscapes_20200607_001014-082fc334.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_80k_cityscapes/upernet_r101_769x769_80k_cityscapes_20200607_001014.log.json)     |

### ADE20K

| Method  | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                 | download                                                                                                                                                                                                                                                                                                                               |
| ------- | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ---------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| UPerNet | R-50     | 512x512   |   80000 | 8.1      | 23.40          | 40.70 |         41.81 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x512_80k_ade20k.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_80k_ade20k/upernet_r50_512x512_80k_ade20k_20200614_144127-ecc8377b.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_80k_ade20k/upernet_r50_512x512_80k_ade20k_20200614_144127.log.json)         |
| UPerNet | R-101    | 512x512   |   80000 | 9.1      | 20.34          | 42.91 |         43.96 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x512_80k_ade20k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_80k_ade20k/upernet_r101_512x512_80k_ade20k_20200614_185117-32e4db94.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_80k_ade20k/upernet_r101_512x512_80k_ade20k_20200614_185117.log.json)     |
| UPerNet | R-50     | 512x512   |  160000 | -        | -              | 42.05 |         42.78 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x512_160k_ade20k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_160k_ade20k/upernet_r50_512x512_160k_ade20k_20200615_184328-8534de8d.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_160k_ade20k/upernet_r50_512x512_160k_ade20k_20200615_184328.log.json)     |
| UPerNet | R-101    | 512x512   |  160000 | -        | -              | 43.82 |         44.85 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x512_160k_ade20k.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_160k_ade20k/upernet_r101_512x512_160k_ade20k_20200615_161951-91b32684.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_160k_ade20k/upernet_r101_512x512_160k_ade20k_20200615_161951.log.json) |

### Pascal VOC 2012 + Aug

| Method  | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                  | download                                                                                                                                                                                                                                                                                                                                   |
| ------- | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| UPerNet | R-50     | 512x512   |   20000 | 6.4      | 23.17          | 74.82 |         76.35 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x512_20k_voc12aug.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_20k_voc12aug/upernet_r50_512x512_20k_voc12aug_20200617_165330-5b5890a7.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_20k_voc12aug/upernet_r50_512x512_20k_voc12aug_20200617_165330.log.json)     |
| UPerNet | R-101    | 512x512   |   20000 | 7.5      | 19.98          | 77.10 |         78.29 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x512_20k_voc12aug.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_20k_voc12aug/upernet_r101_512x512_20k_voc12aug_20200617_165629-f14e7f27.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_20k_voc12aug/upernet_r101_512x512_20k_voc12aug_20200617_165629.log.json) |
| UPerNet | R-50     | 512x512   |   40000 | -        | -              | 75.92 |         77.44 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r50_512x512_40k_voc12aug.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_40k_voc12aug/upernet_r50_512x512_40k_voc12aug_20200613_162257-ca9bcc6b.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_40k_voc12aug/upernet_r50_512x512_40k_voc12aug_20200613_162257.log.json)     |
| UPerNet | R-101    | 512x512   |   40000 | -        | -              | 77.43 |         78.56 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/upernet/upernet_r101_512x512_40k_voc12aug.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_40k_voc12aug/upernet_r101_512x512_40k_voc12aug_20200613_163549-e26476ac.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_40k_voc12aug/upernet_r101_512x512_40k_voc12aug_20200613_163549.log.json) |