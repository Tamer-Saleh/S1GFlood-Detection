<h1 align="center">
  <b>DAM-Net: Global Flood Detection from SAR Imagery Using Differential Attention Metric-Based Vision Transformers</b><br>
</h1>

<h2 align="left">Authors <br></h2>

[![Author](https://img.shields.io/badge/Tamer-Saleh-orange.svg)](https://www.bu.edu.eg/staff/tamermohamed3) 
[![Author](https://img.shields.io/badge/GuiSong-Xia-orange.svg)](http://www.captain-whu.com/xia_En.html) 
[![Author](https://img.shields.io/badge/Shimaa-Holail-orange.svg)](https://www.linkedin.com/in/shimaaholail/) 
[![Author](https://img.shields.io/badge/Xingxing-Weng-orange.svg)]() 
[![Author](https://img.shields.io/badge/Chen-Hao-orange.svg)]() 


## Updates
| :zap:         | March, 2023: DAM-Net has been submitted for publication at ISPRS Journal of Photogrammetry and Remote Sensing. |
|---------------|:------------------------|


## Preamble
The following animation shows SAR images before and after the event and a sample of flooded area findings for a rural area in Iran that was hit by a flood in March 2019. The right figure provides an enlarged visual of a 1 km x 1 km area within the larger area as in the yellow box, showing the size of the affected buildings from the flood by our model.

 <div align="left">
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/test-map.gif" width="480" height="340" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/zoom-test-map.gif" width="340" height="340" />
</div>

## Description

Flooding can cause extensive damage to people, ecosystems, and economies, making it a severe natural disaster. Operating ground-based equipment in flood zones is hazardous, and limited physical access to flooded areas can make it challenging to acquire information about flood extent on the ground. Accurately detecting floods and flood extent via remote sensing greatly aids in mitigating and responding to these events. Remote sensing technology, such as satellites and airborne sensors, can provide valuable information about the extent of flooding, crucial for developing appropriate response strategies and minimizing damages. In this work, we present a new open-source global-scale flood detection dataset, S1GFloods, has been compiled to aid in flood detection. The dataset includes global pairs of high-resolution Sentinel-1 SAR images covering 42 flood events between 2016 and 2022, along with ground truth maps for each pixel. It showcases flooded areas such as rivers, lakes, vegetation, urban and rural areas, and common causes of flooding. This dataset provides critical information for developing strategies to mitigate and respond to future flooding events.
 
 <div align="center">
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Bangladesh-Img.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Iran-Img.gif" width="266" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Nigeria-Img.gif" width="266" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Nanchang-Img.gif" width="133" height="200" />
</div>

 <div align="center">
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Bangladesh-GT.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Iran-GT.gif" width="266" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Nigeria-GT.gif" width="266" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Nanchang-GT.gif" width="133" height="200" />
</div>

 <div align="center">
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Wuhan-Img.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Redrivernorth-Img.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Sudan-Img.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Florence-Img.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Zambia-Img.gif" width="266" height="200" />
</div>

 <div align="center">
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Wuhan-GT.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Redrivernorth-GT.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Sudan-GT.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Florence-GT.gif" width="133" height="200" />
  <img src="https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Zambia-GT.gif" width="266" height="200" />
</div>


| Image Ref. |      Site     | S1 Pre Date  | S1 Post Date |    GT Date   |
| ---------- | ------------- | ------------ | ------------ | ------------ |
|   Img (1)  |   Bangladesh  |  14-03-2017  |  12-07-2017  |  12-07-2017  |
|   Img (2)  |      Iran     |  12-07-2019  |  29-03-2019  |  29-03-2019  |
|   Img (3)  |    Nigeria    |  26-08-2022  |  13-10-2022  |  13-10-2022  |
|   Img (4)  |   Nanchang    |  21-04-2020  |  14-07-2020  |  14-07-2020  |
|   Img (5)  |     Wuhan     |  02-05-2020  |  13-07-2020  |  13-07-2020  |
|   Img (6)  | Redrivernorth |  09-02-2019  |  28-05-2019  |  28-05-2019  |  
|   Img (7)  |     Sudan     |  13-07-2020  |  23-09-2020  |  23-09-2020  |
|   Img (8)  |   Florence    |  21-07-2018  |  19-09-2018  |  19-09-2018  |
|   Img (9)  |     Zambia    |  25-03-2017  |  06-04-2017  |  06-04-2017  |


## Requirements

[![Python 3.7+](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-376/) 
[![Pytorch 1.7.1](https://img.shields.io/badge/Pytorch-1.7.1-blue.svg)](https://pytorch.org/get-started/previous-versions/)
[![torchvision 0.8.2](https://img.shields.io/badge/torchvision-0.8.2-blue.svg)](https://pypi.org/project/torchvision/0.8.2/)
[![Opencv 4.5.5](https://img.shields.io/badge/Opencv-4.5.5-blue.svg)](https://opencv.org/opencv-4-5-5/)
[![CUDA Toolkit 10.1](https://img.shields.io/badge/CUDA-10.1-blue.svg)](https://developer.nvidia.com/cuda-10.1-download-archive-base)
[![Python-SNAPPY 8.0](https://img.shields.io/badge/PythonSNAPPY-8.0-blue.svg)](https://senbox.atlassian.net/wiki/spaces/SNAP/pages/50855941/Configure+Python+to+use+the+SNAP-Python+snappy+interface)
[![Wandb 0.13.10](https://img.shields.io/badge/Wandb-0.13.10-blue.svg)](https://pypi.org/project/wandb/)


## Our model
An overview of the proposed DAM-Net. The feature maps of the pre-and post-event image pairs are extracted through a Siamese structure and pre-trained remote sensing. 
![Overall](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/overall.png)

 
## Quantitative Results
![image-QuantitativeResult](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/table-test.jpg)

## Qualitative Results
A visual comparison of flood detection results in the Iran dataset. The first three images, (a), (b), and (c), represent the pre-flood image, post-flood image, and binary ground truth, respectively. The subsequent images show a comparison of flood detection using various methods, including (d) Unet, (e) FC-Siam-Conc, (f) FC-Siam-Diff, (g) SNUNet-ECAM, (h) Siam-Nested-Unet, (i) ResNet50-IMP, (j) ResNet50-RSP, (k) Swin-T-IMP, (l) ViTAEv2-IMP, (m) Swin-T-RSP, and (n) our proposed DAM-Net method.
![image-QualitativeResult](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Iran-results.png)


### 🔭 Baselines <a name="baselines"></a>

- :open_book:	:open_book:	 :open_book: DTCDSCN [[here](https://ieeexplore.ieee.org/abstract/document/9311793)]
- :open_book:	:open_book:	 :open_book: UNet [[here](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIV-4-W3-2020/215/2020/)]
- :open_book:	:open_book:	 :open_book: FC-Siam [[here](https://ieeexplore.ieee.org/abstract/document/8451652)]
- :open_book:	:open_book:	 :open_book: SNUNet–ECAM [[here](https://ieeexplore.ieee.org/abstract/document/9355573)]
- :open_book:	:open_book:	 :open_book: Siam-Nested-UNet [[here](https://dl.acm.org/doi/abs/10.1145/3437802.3437810)]
- :open_book:	:open_book:	 :open_book: ResNet50-IMP [[here](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)]
- :open_book:	:open_book:	 :open_book: ResNet50-RSP [[here](https://ieeexplore.ieee.org/abstract/document/9782149)]
- :open_book:	:open_book:	 :open_book: Swin–T-RSP [[here](https://ieeexplore.ieee.org/abstract/document/9782149)]
- :open_book:	:open_book:	 :open_book: Swin-T-IMP [[here](https://ieeexplore.ieee.org/abstract/document/9736956)]
- :open_book:	:open_book:	 :open_book: ViTAEv2 [[here](https://arxiv.org/pdf/2202.10108.pdf)]


## :speech_balloon: <span id="jump">Dataset Preparation</span>

### :point_right: Data Structure

```yaml
For S1GFloods dataset, clip the images to 256 × 256 patches. Please, respect the following structure: 
├————train/
|      ├———Pre/                                  Images of Time 1 before the flood event
            ├———<region><year><XY>.png
            ...
            ├———<region><year><XY>.png
|      ├———Post/                                 Images of Time 2 after the flood event
            ├———<region><year><XY>.png
            ...
            ├———<region><year><XY>.png            
|      ├———GT/                                   Ground truth labels
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|
├————val/
|      ├———Pre/  
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———Post/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———GT/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|
├————test/
|      ├———Pre/  
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———Post/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———GT/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
```

### :truck: Datasets <a name="dataset"></a>

The full train and test code will be released soon. You can download our novel public S1GFloods dataset through the following link:

- [x] [S1GFloods][baidu drive](https://pan.baidu.com/s/1-8BFn1PmguxiP1RoLwbOCA) Passward: (gjwc)

### :page_with_curl: Citing <a name="citing"></a>

```bibtex
@ARTICLE{tamersalehdam2023,
  Author = {T. Saleh, G-S Xia, S. Holail, X. Weng, and C. Hao},
  Title = {DAM-Net: Global Flood Detection from SAR Imagery Using Differential Attention Metric-Based Vision Transformers},
  Journal = {ISPRS Journal of Photogrammetry and Remote Sensing},
  Year = {2023},
  volume={},
  number={},
  pages={1-21}
  }
```

  
## Contact Information

If you have any questions or would like to collaborate, please reach out to me at tamersaleh@whu.edu.cn or feel free to make issues.

## License
The code and datasets are released for non-commercial and research purposes only. For commercial purposes, please contact the authors.


## Acknowledgment

Appreciate the work from the following repositories:

- [wenhwu/awesome-remote-sensing-change-detection](https://github.com/wenhwu/awesome-remote-sensing-change-detection)
- [SNUNet-CD](https://github.com/RSCD-Lab/Siam-NestedUNet)
- [BIT-CD](https://github.com/justchenhao/BIT_CD)

## Related resources
- [ASF-Dataset](https://search.asf.alaska.edu/)
- [Sentinel-Hub](https://scihub.copernicus.eu/)
- [SNAP Toolbox](http://step.esa.int/main/download/)



