<h1 align="center">
  <b>DAM-Net: Global Flood Detection from SAR Imagery Using Differential Attention Metric-Based Vision Transformers</b><br>
</h1>

[`Tamer Saleh`](https://www.bu.edu.eg/staff/tamermohamed3), [`Gui-Song Xia`](http://www.captain-whu.com/xia_En.html), [`Shimaa Holail Researchgate`](https://www.researchgate.net/profile/Shimaa-Holail)[`Shimaa Holail Linkedin`](https://www.linkedin.com/in/shimaaholail/), [`Xingxing Weng`], and [`Chen Hao`]

The train and test code will be released soon. The S1GFloods dataset is available. 


## Updates
| :zap:         | DAM-Net has been submitted for publication at ISPRS Journal of Photogrammetry and Remote Sensing. |
|---------------|:------------------------|



## :speech_balloon: S1GFloods Dataset 
Flooding is a severe natural disaster that can cause extensive damage to people, ecosystems, and economies. The impact of floods can be catastrophic, and a single major flood event can result in billions of dollars in damages. However, the hazards of operating ground-based equipment in flood zones and the limited physical access to flooded areas make it difficult to acquire information about flood extent on the ground. Accurately detecting floods and flood extent via remote means greatly aids in the process of mitigating and responding to these destructive events. Remote sensing technology, including satellites and airborne sensors, can provide valuable information about the extent of flooding, which is crucial for developing appropriate response strategies and minimizing damages. By using remote sensing technology, scientists, government agencies, and emergency responders can effectively assess the situation and develop strategies to minimize the damage caused by flooding events.

 
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



## :speech_balloon: Network Architecture
An overview of the proposed DAM-Net. The feature maps of the pre-and post-event image pairs are extracted through a Siamese structure and pre-trained remote sensing. 
![Overall](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/overall.png)


 ## :speech_balloon: <span id="jump">Quantitative and Qualitative Results on the testing set of SIGFloods Dataset</span>
 
### :point_right: Quantitative Results
![image-QuantitativeResult](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/table-test.jpg)

### :point_right: Qualitative Results
A visual comparison of flood detection results in the Iran dataset. The first three images, (a), (b), and (c), represent the pre-flood image,
post-flood image, and binary ground truth, respectively. The subsequent images show a comparison of flood detection using various
methods, including (d) Unet, (e) FC-Siam-Conc, (f) FC-Siam-Diff, (g) SNUNet-ECAM, (h) Siam-Nested-Unet, (i) ResNet50-IMP,
(j) ResNet50-RSP, (k) Swin-T-IMP, (l) ViTAEv2-IMP, (m) Swin-T-RSP, and (n) our proposed DAM-Net method.
![image-QualitativeResult](https://github.com/Tamer-Saleh/GFlood-Detection/blob/Flood-Mapping/images/Iran-results.png)


## :speech_balloon: Requirements

- Python 3.7
- Pytorch 1.7

Please see `requirements.txt` for all the other requirements.


### 🔭 Baselines <a name="baselines"></a>

- [x] DTCDSCN [[paper](https://ieeexplore.ieee.org/abstract/document/9311793)]
- [x] UNet [[paper](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIV-4-W3-2020/215/2020/)]
- [x] FC-Siam [[paper](https://ieeexplore.ieee.org/abstract/document/8451652)]
- [x] SNUNet–ECAM [[paper](https://ieeexplore.ieee.org/abstract/document/9355573)]
- [x] Siam-Nested-UNet [[paper](https://dl.acm.org/doi/abs/10.1145/3437802.3437810)]
- [x] ResNet50-IMP [[paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)]
- [x] ResNet50-RSP [[paper](https://ieeexplore.ieee.org/abstract/document/9782149)]
- [x] Swin–T-RSP [[paper](https://ieeexplore.ieee.org/abstract/document/9782149)]
- [x] Swin-T-IMP [[paper](https://ieeexplore.ieee.org/abstract/document/9736956)]
- [x] ViTAEv2 [[paper](https://arxiv.org/pdf/2202.10108.pdf)]




#### Encoders <a name="encoders"></a>

Below is a list of encoders used in this work and their pre-trained weights.

<details>
<summary style="margin-left: 25px;">ResNet</summary>
<div style="margin-left: 25px;">

| Encoder   |        Weights        | Params, M |
| --------- | :-------------------: | :-------: |
| resnet50  | imagenet / ssl / swsl |    23M    |
| resnet101 |       imagenet        |    42M    |


</div>
</details>

<details>
<summary style="margin-left: 25px;">RegNet(x/y)</summary>
<div style="margin-left: 25px;">

| Encoder          | Weights  | Params, M |
| ---------------- | :------: | :-------: |
| timm-regnety_120 | imagenet |    49M    |
| timm-regnety_160 | imagenet |    80M    |
| timm-regnety_320 | imagenet |   141M    |


</div>
</details>


## :speech_balloon: <span id="jump">Dataset Preparation</span>

### :point_right: Data Structure

```
"""
EGY-BCD dataset with pixel-level binary labels；
├————train
|      ├———A  
|      ├———B
|      ├———label
|
├————val
|      ├———A  
|      ├———B
|      ├———label
|
├————test
|      ├———A  
|      ├———B
|      ├———label
"""
```

`A`: Images of Time1;
`B`:Images of Time2;
`label`: Ground Truth;
`each file contains the image names (XXXX.png)`


### :truck: Datasets <a name="dataset"></a>

You can download our novel public EGY-BCD dataset through the following link:

- [x] [EGY-BCD][baidu drive](https://pan.baidu.com/s/1DW3pfwQn3W4zYkYfCBCCdw) Passward: (ef21)


### :page_with_curl: Citing <a name="citing"></a>

```
@ARTICLE{shimaabuilding2023,
  Author = {S. Holail, T. Saleh, X. Xiao, and D. Li},
  Title = {AFDE-Net: Building Change Detection using Attention-Based Feature Differential Enhancement for Satellite Imagery},
  Journal = {IEEE Geoscience and Remote Sensing Letters},
  Year = {2023},
  volume={},
  number={},
  pages={1-5}
  }
```
  
### Contact Information
If you have any question about EGY-BCD dataset, please contact shimaaholail@whu.edu.cn


## :speech_balloon: References

Appreciate the work from the following repositories:

- [wenhwu/awesome-remote-sensing-change-detection](https://github.com/wenhwu/awesome-remote-sensing-change-detection)
- [qubvel/segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch)
- [likyoo/PRCV2021_ChangeDetection_Top3](https://github.com/likyoo/PRCV2021_ChangeDetection_Top3)
- [likyoo/Pytorch-UNet](https://github.com/likyoo/Pytorch-UNet)
- [angup143/disaster_mapping](https://github.com/angup143/disaster_mapping/tree/5bab37700950bb9b5e6af9bbe41a6ab66645bf58)


