# Multimodal Remote Sensing Segmentation Models

A categorized catalog of multimodal remote sensing segmentation models, organized by the challenge they primarily address. Compiled from the *Classification of Multimodal Remote Sensing Models* table. This article has been submitted to the journal **Computers & Geosciences**.

**81 models** across **6 categories** and **18 sub-categories**.

> **A note on the links below:** Each model name below links to a Google Scholar search for its exact paper title, which gets you to the paper  in one click.

## Table of Contents

- [Complex Landscapes & Environmental Variations](#complex-landscapes--environmental-variations)
  - [Urban & Building Extraction](#urban--building-extraction)
  - [Agricultural Landscape Mapping](#agricultural-landscape-mapping)
  - [Cloud & Occlusion Handling](#cloud--occlusion-handling)
- [Segmentation Accuracy](#segmentation-accuracy)
  - [Edge & Detail Preservation](#edge--detail-preservation)
  - [C2Seg Challenge](#c2seg-challenge)
- [Scalability & Real-Time Decision Making](#scalability--real-time-decision-making)
  - [Resource-efficient Lightweight Architectures](#resource-efficient-lightweight-architectures)
  - [Data Fusion Techniques](#data-fusion-techniques)
- [Data & Sensor Limitations](#data--sensor-limitations)
  - [Data Acquisition & Availability](#data-acquisition--availability)
  - [Limitations of Single Modalities](#limitations-of-single-modalities)
  - [Data Heterogeneity](#data-heterogeneity)
  - [Fusion Techniques](#fusion-techniques)
  - [Class Imbalance](#class-imbalance)
- [Semantic Gap](#semantic-gap)
  - [Specialized Datasets](#specialized-datasets)
  - [Vision-Language Model Adaptation](#vision-language-model-adaptation)
  - [Precision Alignment](#precision-alignment)
  - [Feature Fusion](#feature-fusion)
- [Robustness](#robustness)
  - [Data Integration & Modality Discrepancies](#data-integration--modality-discrepancies)
  - [Environmental Variations & Conditions](#environmental-variations--conditions)

---

## Complex Landscapes & Environmental Variations

### Urban & Building Extraction

| Model | Modalities | Datasets & Rankings | Reference | Github |
|---|---|---|---|---|
| [MFFN](https://scholar.google.com/scholar?q=A+Multimodal+Feature+Fusion+Network+for+Building+Extraction+With+Very+High-Resolution+Remote+Sensing+Image+and+LiDAR+Data) | HRI & LiDAR | IoU (Vaihingen 91.8%, Potsdam 93.04%, USGS 84.59%) | Luo et al., 2024 |
| [UisNet](https://scholar.google.com/scholar?q=Fine-scale+urban+informal+settlements+mapping+by+fusing+remote+sensing+images+and+building+data+via+a+transformer-based+multimodal+fusion+network) | RGB & Building Polygon | mIoU (Shenzhen 85.51%, GID 60.23%) | Fan et al., 2022 | https://github.com/RunyuFan/|
| [PMNet](https://scholar.google.com/scholar?q=A+point-wise+LiDAR+and+image+multimodal+fusion+network+%28PMNet%29+for+aerial+point+cloud+3D+semantic+segmentation) | HSI & LiDAR | mIoU (UHC 71%, Osaka 57%) | Poliyapram et al., 2019 |

### Agricultural Landscape Mapping

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [CM-Net](https://scholar.google.com/scholar?q=Cross-Modal+Segmentation+Network+for+Winter+Wheat+Mapping+in+Complex+Terrain+Using+Remote-Sensing+Multi-Temporal+Images+and+DEM+Data) | MSI & DEM | mIoU (Wheat 89.60%) | Wang et al., 2024 |
| [TMFNet](https://scholar.google.com/scholar?q=A+Transformer-based+multi-modal+fusion+network+for+semantic+segmentation+of+high-resolution+remote+sensing+imagery) | MSI & nDSM | mIoU (Vaihingen 78.70%, Potsdam 85.67%) | Liu et al., 2024 |

### Cloud & Occlusion Handling

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [CloudSeg](https://scholar.google.com/scholar?q=CloudSeg%3A+A+multi-modal+learning+framework+for+robust+land+cover+mapping+under+cloudy+conditions) | RGB & NIR & SAR | mIoU (M3M-CR 53.64%, WHU-OPT-SAR 52.40%) | Xu et al., 2024 |
| [MoCG](https://scholar.google.com/scholar?q=MoCG%3A+Modality+Characteristics-Guided+Semantic+Segmentation+in+Multimodal+Remote+Sensing+Images) | OPT & SAR | mIoU (WHU-OPT-SAR 69.1%, DFC23 86.7%) | Xiao et al., 2023 |

---

## Segmentation Accuracy

### Edge & Detail Preservation

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [DEFLNet](https://scholar.google.com/scholar?q=High-Resolution+Remote+Sensing+Image+Segmentation+Based+on+Efficient+Dual-Modal+Feature+Learning) | IRRG & DSM | OA (Vaihingen 90.45%, Potsdam 94.52%) | Zhang et al., 2024 |
| [DFCN](https://scholar.google.com/scholar?q=Densely+based+multi-scale+and+multi-modal+fully+convolutional+networks+for+high-resolution+remote-sensing+image+semantic+segmentation) | RGB & nDSM | OA (Vaihingen 89.24%, Potsdam 89.95%) | Peng et al., 2019 |
| [PACSCNet](https://scholar.google.com/scholar?q=Progressive+adjacent-layer+coordination+symmetric+cascade+network+for+semantic+segmentation+of+multimodal+remote+sensing+images) | IRRG & nDSM | mIoU (Vaihingen 82.25%, Potsdam 76.03%) | Fan et al., 2024 |
| [MGFNet](https://scholar.google.com/scholar?q=MGFNet%3A+An+MLP-dominated+gated+fusion+network+for+semantic+segmentation+of+high-resolution+multi-modal+remote+sensing+images) | OPT & SAR | mIoU (YESeg-OPT-SAR 71.21%, Pohang 84.37%) | Wei et al., 2024 |
| [DFFNet](https://scholar.google.com/scholar?q=Based+on+multi-feature+information+attention+fusion+for+multi-modal+remote+sensing+image+semantic+segmentation) | IRRG & DSM | mIoU (Vaihingen 82.47%) | Zhang, 2021 |
| [FDGSNet](https://scholar.google.com/scholar?q=FDGSNet%3A+A+Multi-modal+Gated+Segmentation+Network+for+Remote+Sensing+Image+Based+on+Frequency+Decomposition) | IRRGB & DSM | mIoU (Potsdam 86.34%) | Cui et al., 2024 |

### C2Seg Challenge

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [MUDARSIS](https://scholar.google.com/scholar?q=Multimodal+unsupervised+domain+adaptation+for+remote+sensing+image+segmentation) | MSI & HSI & SAR | mIoU (C2Seg 0.1851%) | Zou et al., 2023 |
| [MRSN](https://scholar.google.com/scholar?q=Multimodal+Remote+Sensing+Network) | MSI & HSI & SAR | mIoU (C2Seg 0.1387%) | Zhao et al., 2023 |
| [MMGLOTS](https://scholar.google.com/scholar?q=MMGLOTS%3A+Multi-Modal+Global-Local+Transformer+Segmentor+for+Remote+Sensing+Image+Segmentation) | MSI & HSI & SAR | mIoU (C2Seg 0.1988%) | Liu et al., 2023 |

---

## Scalability & Real-Time Decision Making

### Resource-efficient Lightweight Architectures

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [STONet-S](https://scholar.google.com/scholar?q=STONet-S%2A%3A+A+Knowledge-Distilled+Approach+for+Semantic+Segmentation+in+Remote-Sensing+Images) | IRRG & nDSM | mIoU (Vaihingen 81.40%, Potsdam 76.17%) | Zhou et al., 2024 |
| [C3Net](https://scholar.google.com/scholar?q=C3net%3A+Cross-modal+feature+recalibrated%2C+cross-scale+semantic+aggregated+and+compact+network+for+semantic+segmentation+of+multi-modal+high-resolution+aerial+images) | IRRG & DSM | OA (Vaihingen 91.3%) | Cao et al., 2021 |
| [MM_MT](https://scholar.google.com/scholar?q=Multi-task+Learning+of+Semantic+Segmentation+and+Height+Estimation+for+Multi-modal+Remote+Sensing+Images) | RGB & IR | mIoU (Potsdam 83.02%) | Mengyu et al., 2024 |

### Data Fusion Techniques

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [MFTransNet](https://scholar.google.com/scholar?q=MFTransNet%3A+a+multi-modal+fusion+with+CNN-transformer+network+for+semantic+segmentation+of+HSR+remote+sensing+images) | RGB & DSM | mIoU (Potsdam 72.34%) | He et al., 2023 |
| [Beyond RGB](https://scholar.google.com/scholar?q=Beyond+RGB%3A+Very+high+resolution+urban+remote+sensing+with+multimodal+deep+networks) | IRRG & nDSM | OA (Vaihingen 90.3%, Potsdam 90.6%) | Audebert et al., 2018 |
| [LMFNet](https://scholar.google.com/scholar?q=LMFNet%3A+An+Efficient+Multimodal+Fusion+Approach+for+Semantic+Segmentation+in+High-Resolution+Remote+Sensing) | MSI & DSM | mIoU (US3D 85.09%, Vaihingen 82.49%, Potsdam 86.39%) | Wang et al., 2024 |
| [LMF-Net](https://scholar.google.com/scholar?q=LMF-Net%3A+A+Learnable+Multi-modal+Fusion+Network+for+Semantic+Segmentation+of+Remote+Sensing+Data) | OPT & DSM | mIoU (Vaihingen 83.15%, Potsdam 86.83%) | Li et al., 2025 |
| [MultiSenseSeg](https://scholar.google.com/scholar?q=MultiSenseSeg%3A+A+cost-effective+unified+multimodal+semantic+segmentation+model+for+remote+sensing) | RGB & IRRG & DSM | OA (Potsdam 87.13%) | Wang et al., 2024 |

---

## Data & Sensor Limitations

### Data Acquisition & Availability

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [SM-GANs](https://scholar.google.com/scholar?q=Multimodal+GANs%3A+Toward+crossmodal+hyperspectral--multispectral+image+segmentation) | MSI & HSI | mIoU (Pavia 75.92%, LCZ 51.01%) | Hong et al., 2020 |
| [FTransUNet](https://scholar.google.com/scholar?q=A+multilevel+multimodal+fusion+transformer+for+remote+sensing+semantic+segmentation) | NIRRG & IRRGB & nDSM | mIoU (Vaihingen 84.23%, Potsdam 86.20%) | Ma et al., 2024 |

### Limitations of Single Modalities

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [RSCNN](https://scholar.google.com/scholar?q=Deep+semantic+segmentation+of+aerial+imagery+based+on+multi-modal+data) | IRRG & nDSM | mIoU (Vaihingen 60.89%) | Chen et al., 2018 |
| [CMFNet](https://scholar.google.com/scholar?q=A+crossmodal+multiscale+fusion+network+for+semantic+segmentation+of+remote+sensing+data) | RGB & DSM | mIoU (Vaihingen 81.44%, Potsdam 85.63%) | Ma et al., 2022 |
| [AMBNet](https://scholar.google.com/scholar?q=AMBNet%3A+Adaptive+Multi-feature+Balanced+Network+for+Multimodal+Remote+Sensing+Semantic+Segmentation) | RGB & DSM | mIoU (Vaihingen 83.41%, Potsdam 83.33%) | Xiu et al., 2024 |

### Data Heterogeneity

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [IML](https://scholar.google.com/scholar?q=A+Novel+Approach+to+Incomplete+Multimodal+Learning+for+Remote+Sensing+Data+Fusion) | RGB & SAR & nDSM | mIoU (DFC2023 85.8%) | Chen et al., 2024 |
| [CMMSNet](https://scholar.google.com/scholar?q=CMMSNet%3A+A+Multi-modal+Semantic+Segmentation+Network+for+Rooftop+Extraction+based+on+SAR+and+Optical+Images) | OPT & SAR | IoU (DFC2023 85.8%) | Shen et al., 2024 |
| [SSMF](https://scholar.google.com/scholar?q=Multi-modal+deep+learning+approaches+to+semantic+segmentation+of+mining+footprints+with+multispectral+satellite+imagery) | RGB & NIR | mIoU (SSMF 72.71%) | Saputra et al., 2025 |

### Fusion Techniques

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [VSGNet](https://scholar.google.com/scholar?q=Vision+foundation+model+guided+multi-modal+fusion+network+for+remote+sensing+semantic+segmentation) | RGB & nDSM | mIoU (Potsdam 90.02%, Vaihingen 84.77%) | Pan et al., 2024 |
| [MFNet](https://scholar.google.com/scholar?q=Deep+multimodal+fusion+network+for+semantic+segmentation+using+remote+sensing+image+and+LiDAR+data) | IRRG & nDSM | mIoU (Potsdam 91.8%, Vaihingen 91.3%, GRSS DFC Zeebrugge 88.87%) | Sun et al., 2021 |
| [MCANet](https://scholar.google.com/scholar?q=MCANet%3A+A+joint+semantic+segmentation+framework+of+optical+and+SAR+images+for+land+use+classification) | OPT & SAR | OA (WHU-OPT-SAR 82.9%) | Li et al., 2022 |
| [CaFE](https://scholar.google.com/scholar?q=Category-wise+fusion+and+enhancement+learning+for+multimodal+remote+sensing+image+semantic+segmentation) | RGB & DSM | mIoU (Potsdam 85.26%, Vaihingen 81.07%) | Zheng et al., 2022 |
| [IKD-Net](https://scholar.google.com/scholar?q=Imbalance+knowledge-driven+multi-modal+network+for+land-cover+semantic+segmentation+using+aerial+images+and+LiDAR+point+clouds) | RGB & LiDAR | mIoU (N3C-California 75.50%) | Wang et al., 2023 |
| [AMIANet](https://scholar.google.com/scholar?q=AMIANet%3A+Asymmetric+Multimodal+Interactive+Augmentation+Network+for+Semantic+Segmentation+of+Remote+Sensing+Imagery) | RGB & LiDAR | mIoU (N3C-California 78.13%, WHU-RRDSD 67.51%, Vaihingen 75.69%) | Liu et al., 2024 |
| [SkySense](https://scholar.google.com/scholar?q=Skysense%3A+A+multi-modal+remote+sensing+foundation+model+towards+universal+interpretation+for+earth+observation+imagery) | OPT & MSI & SAR | mIoU (DynamicEarthNet-MM 70.91%) | Guo et al., 2024 |
| [MFMamba](https://scholar.google.com/scholar?q=MFMamba%3A+A+Mamba-Based+Multi-Modal+Fusion+Network+for+Semantic+Segmentation+of+Remote+Sensing+Images) | NIRRG & RGB & DSM | mIoU (Potsdam 86.12%, Vaihingen 83.13%) | Wang et al., 2024 |
| [Mamba-diffusion](https://scholar.google.com/scholar?q=A+Mamba-Diffusion+Framework+for+Multimodal+Remote+Sensing+Image+Semantic+Segmentation) | OPT & SAR | mIoU (WHU-OPT-SAR 59.21%, Hunan 53.06%) | Du et al., 2024 |
| [ASMFNet](https://scholar.google.com/scholar?q=Adjacent-Scale+Multimodal+Fusion+Networks+for+Semantic+Segmentation+of+Remote+Sensing+Data) | OPT & DSM | mIoU (Potsdam 85.34%, Vaihingen 80.47%) | Ma et al., 2024 |
| [EMSNet](https://scholar.google.com/scholar?q=EMSNet%3A+Efficient+Multimodal+Symmetric+Network+for+Semantic+Segmentation+of+Urban+Scene+from+Remote+Sensing+Imagery) | NIRRGB & IRRGB & DSM & SAR | mIoU (Potsdam 82.7%, Vaihingen 70.2%, WHU-Opt-Sar 49.1%, DFC2023 77.1%) | Zhou et al., 2025 |
| [DF2RQ](https://scholar.google.com/scholar?q=DF+2+RQ%3A+Dynamic+Feature+Fusion+via+Region-wise+Queries+for+Semantic+Segmentation+of+Multimodal+Remote+Sensing+Data) | RGB & SAR & DEM & NDVI<br>SAR & HSI & MSI<br>NIRRG & DSM<br>IRRGB & DSM | mIoU (Globe230k 80.73%)<br>mIoU (C2Seg-BW 15.13%)<br>mIoU (Vaihingen 85.02%)<br>mIoU (Potsdam 88.12%) | Feng et al., 2025 |
| [DLLR](https://scholar.google.com/scholar?q=Difference-complementary+Learning+and+Label+Reassignment+for+Multimodal+Semi-Supervised+Semantic+Segmentation+of+Remote+Sensing+Images) | OPT & SAR | mIoU (WHU-OPT-SAR 62.47%) | Han et al., 2025 |

### Class Imbalance

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [PerceiverIO](https://scholar.google.com/scholar?q=General-purpose+multimodal+transformer+meets+remote+sensing+semantic+segmentation) | RGIR & RGBIR & nDSM<br>SAR & DEM | mIoU (Vaihingen 60%, Potsdam 63%)<br>mIoU (MMFlood 58%) | Kieu et al., 2023 |

---

## Semantic Gap

### Specialized Datasets

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [RISRSD](https://scholar.google.com/scholar?q=Referring+Image+Segmentation+for+Remote+Sensing+Data) | RSI & RE | mIoU (SkyScapes 57.74%) | Yuan et al., 2024 |
| [RefSegRS](https://scholar.google.com/scholar?q=Rrsis%3A+Referring+remote+sensing+image+segmentation) | RSI & RE | mIoU (RefSegRS 59.96%) | Yuan et al., 2024 |
| [RMSIN](https://scholar.google.com/scholar?q=Rotated+multi-scale+interaction+network+for+referring+remote+sensing+image+segmentation) | RSI & RE | mIoU (RRSIS-D 64.20%) | Liu et al., 2024 |
| [RISBench](https://scholar.google.com/scholar?q=Cross-Modal+Bidirectional+Interaction+Model+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 64.46%, RefSegRS 59.77%, RISBench 69.33%) | Dong et al., 2024 |
| [CADFormer](https://scholar.google.com/scholar?q=CADFormer%3A+Fine-Grained+Cross-modal+Alignment+and+Decoding+Transformer+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 63.77%, RRSIS-HR 53.29%) | Liu et al., 2025 |
| [CCFormer](https://scholar.google.com/scholar?q=RRSECS%3A+Referring+remote+sensing+expression+comprehension+and+segmentation) | RSI & RE | mIoU (RefDIOR 71.6%) | Lu et al., 2025 |
| [GeoPix](https://scholar.google.com/scholar?q=GeoPix%3A+Multi-Modal+Large+Language+Model+for+Pixel-level+Image+Understanding+in+Remote+Sensing) | RSI & RE | mIoU (GeoPixInstruct 84.25%) | Ou et al., 2025 |
| [AeroReformer](https://scholar.google.com/scholar?q=AeroReformer%3A+Aerial+Referring+Transformer+for+UAV-based+Referring+Image+Segmentation) | RSI & RE | mIoU (UAVid-RIS 72.79%, VDD-RIS8 80.72%) | Li, 2025 |

### Vision-Language Model Adaptation

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [MetaSegNet](https://scholar.google.com/scholar?q=MetaSegNet%3A+Metadata-collaborative+Vision-Language+Representation+Learning+for+Semantic+Segmentation+of+Remote+Sensing+Images) | RSI & RE | mIoU (OpenEarthMap 70.40%, Potsdam 87.60%, LoveDA 52%) | Wang et al., 2024 |
| [SegCLIP](https://scholar.google.com/scholar?q=Segclip%3A+Multimodal+visual-language+and+prompt+learning+for+high-resolution+remote+sensing+semantic+segmentation) | RSI & RE | mIoU (LoveDA 57.98%, iSAID 67.78%, UAVid 75.73%) | Zhang et al., 2024 |
| [MMF-CLIP](https://scholar.google.com/scholar?q=MMF-CLIP%3A+An+Image-Text+Multimodal+Semantic+Segmentation+Method+for+Remote+Sensing+Images) | RSI & RE | mIoU (Potsdam 79.62%) | Yang et al., 2024 |
| [GeoPixel-FT](https://scholar.google.com/scholar?q=GeoPixel%3A+Pixel+Grounding+Large+Multimodal+Model+in+Remote+Sensing) | RSI & RE | mIoU (RRSIS-D 67.30%) | Shabbir et al., 2025 |
| [MANet](https://scholar.google.com/scholar?q=MANet%3A+Fine-Tuning+Segment+Anything+Model+for+Multimodal+Remote+Sensing+Semantic+Segmentation) | NIRRG & RGB & DSM & RE | mIoU (Potsdam 86.69%, Vaihingen 85.03%) | Ma et al., 2024 |
| [RingMoSAM](https://scholar.google.com/scholar?q=RingMo-SAM%3A+A+foundation+model+for+segment+anything+in+multimodal+remote-sensing+images) | OPT & SAR & RE | mIoU (iSAID 57.99%, Vaihingen 72.44%, Potsdam 78.21%, PolSAR-ZG 51%) | Yan et al., 2023 |
| [RS2-SAM 2](https://scholar.google.com/scholar?q=Customized+SAM+2+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 66.72%, RefSegRS 73.9%) | Rong et al., 2025 |
| [PSLG-SAM](https://scholar.google.com/scholar?q=Semantic+Localization+Guiding+Segment+Anything+Model+For+Reference+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 70.61%, RRSIS-M 67.04%) | Li et al., 2025 |
| [BTDNet](https://scholar.google.com/scholar?q=Referring+Remote+Sensing+Image+Segmentation+via+Bidirectional+Alignment+Guided+Joint+Prediction) | RSI & RE | mIoU (RRSIS-D 66.04%, RefSegRS 67.95%) | Zhang et al., 2025 |
| [LSCF](https://scholar.google.com/scholar?q=LSCF%3A+Long-term+Semantic-guidance+ConvFormer+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 64.25%, RefSegRS 77.44%, RISBench 68.53%) | Ma et al., 2025 |
| [RSSep](https://scholar.google.com/scholar?q=RSSep%3A+Sequence-to-Sequence+Model+for+Simultaneous+Referring+Remote+Sensing+Segmentation+and+Detection) | RSI & RE | mIoU (RRSIS-D 69.23%) | Ho et al., 2024 |
| [DiffRIS](https://scholar.google.com/scholar?q=DiffRIS%3A+Enhancing+Referring+Remote+Sensing+Image+Segmentation+with+Pre-trained+Text-to-Image+Diffusion+Models) | RSI & RE | mIoU (RRSIS-D 62.19%, RefSegRS 62.38%, RISBench 67.04%) | Dong et al., 2025 |
| [RSRefSeg](https://scholar.google.com/scholar?q=RSRefSeg%3A+Referring+Remote+Sensing+Image+Segmentation+with+Foundation+Models) | RSI & RE | gIoU (RRSIS-D 64.67%) | Chen et al., 2025 |
| [RSRefSeg2](https://scholar.google.com/scholar?q=RSRefSeg+2%3A+Decoupling+Referring+Remote+Sensing+Image+Segmentation+with+Foundation+Models) | RSI & RE | gIoU (RRSIS-D 69.17%, RefSegRS 77.39%, RISBench 72.57%) | Chen et al., 2025 |
| [FLAVARS](https://scholar.google.com/scholar?q=FLAVARS%3A+A+Multimodal+Foundational+Language+and+Vision+Alignment+Model+for+Remote+Sensing) | RSI & RE | mIoU (SkyScript-Grounded 78.10%) | Corley et al., 2025 |

### Precision Alignment

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [DANet](https://scholar.google.com/scholar?q=Rethinking+the+Implicit+Optimization+Paradigm+with+Dual+Alignments+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 66.07%, RefSegRS 62.14%) | Pan et al., 2024 |
| [FIANet](https://scholar.google.com/scholar?q=Exploring+fine-grained+image-text+alignment+for+referring+remote+sensing+image+segmentation) | RSI & RE | mIoU (RRSIS-D 64.01%, RefSegRS 68.67%) | Lei et al., 2024 |
| [SBANet](https://scholar.google.com/scholar?q=Scale-wise+Bidirectional+Alignment+Network+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 65.52%, RefSegRS 62.73%) | Li et al., 2025 |
| [SUAS](https://scholar.google.com/scholar?q=Semantic+Uncertainty-Awared+for+Semantic+Segmentation+of+Remote+Sensing+Images) | RSI & RE | mIoU (RRSIS-D 65.05%) | Qiu et al., 2025 |

### Feature Fusion

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [MSCMFN](https://scholar.google.com/scholar?q=Mixed-scale+cross-modal+fusion+network+for+referring+image+segmentation) | RSI & RE | mIoU (RRSIS-D 64.20%, RefSegRS 64.73%) | Pan et al., 2025 |
| [BEMSeg](https://scholar.google.com/scholar?q=Bidirectional+feature+fusion+and+enhanced+alignment+based+multimodal+semantic+segmentation+for+remote+sensing+images) | RSI & RE | mIoU (Potsdam 79.33%, Vaihingen 76.28%, LoveDA 54.71%) | Liu & Wang, 2024 |
| [MAFN](https://scholar.google.com/scholar?q=Multimodal-Aware+Fusion+Network+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 64.76%) | Shi & Zhang, 2025 |
| [MPBF](https://scholar.google.com/scholar?q=Multimodal+Prompt-Guided+Bidirectional+Fusion+for+Referring+Remote+Sensing+Image+Segmentation) | RSI & RE | mIoU (RRSIS-D 65.32%) | Li et al., 2025 |

---

## Robustness

### Data Integration & Modality Discrepancies

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [TMCNet](https://scholar.google.com/scholar?q=Tuple+Perturbation-based+Contrastive+Learning+Framework+for+Multimodal+Remote+Sensing+Image+Semantic+Segmentation) | OPT & SAR | OA (YESeg-OPT-SAR 79.82%, WHU-OPT-SAR 82.79%) | Ye et al., 2025 |
| [MIEFNet](https://scholar.google.com/scholar?q=Elevation+information-guided+multimodal+fusion+robust+framework+for+remote+sensing+image+segmentation) | OPT & DSM | mIoU (Vaihingen 85.06%, Potsdam 87.60%) | Fan et al., 2024 |

### Environmental Variations & Conditions

| Model | Modalities | Datasets & Rankings | Reference |
|---|---|---|---|
| [DHRLVR](https://scholar.google.com/scholar?q=Towards+robust+semantic+segmentation+of+land+covers+in+foggy+conditions) | RGB & DSM | OA (Vaihingen 90.49%, Potsdam 90.17%) | Shi et al., 2022 |
| [LRMRRLCCF](https://scholar.google.com/scholar?q=Learning+rich+multimodal+representation+for+robust+land+cover+classification+in+fog) | RGB & DSM | OA (Potsdam 90.91%) | Shi et al., 2024 |

---

## Legend

- **mIoU** — mean Intersection over Union
- **IoU** — Intersection over Union
- **OA** — Overall Accuracy
- **gIoU** — generalized Intersection over Union

