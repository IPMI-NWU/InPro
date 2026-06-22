# ConFus: Consensus Fusion Pseudo-Label Framework with Introspective Prototype for Gaze-Supervised Cardiac Segmentation

> Creating fully annotated labels for medical image segmentation remains both time-consuming and expensive, underscoring the necessity for innovative strategies that reduce dependence on dense annotations. Cardiac segmentation is an essential step in cardiovascular disease diagnosis, but generating fully annotated labels remains time-consuming and expensive, underscoring the need for innovative strategies that reduce reliance on dense annotations. Eye-tracking provides a cost-effective source of supervision that can be seamlessly integrated into radiologists’ workflows without imposing additional annotation burdens. Gaze signals implicitly encode diagnostic attention, providing weak yet semantically informative cues for model optimization. Nevertheless, in multi-class segmentation settings, the inherent sparsity and ambiguity of gaze substantially degrade the quality of supervision, leading to class diffusion and inaccurate segmentation in spatially adjacent regions. To address these challenges, we propose the Consensus Fusion Pseudo-Label Framework (ConFus) for gaze-supervised cardiac segmentation. To mitigate the ambiguity in gaze, the Consensus Fusion Pseudo-Label module deduces labels for uncertain regions via multi-prototype consensus and enhances supervisory signals. To suppress noise from gaze, we design an Introspective Prototype Construction module, which constructs reliable prototypes by exploiting similarity queries across inter-view features with an introspective matching strategy. Finally, the Prototype-centric Contrastive Learning is employed to maximize inter-class feature separability and strengthen discrimination between neighboring anatomical structures. Experimental results on two public cardiac datasets and two public general medical datasets demonstrate that ConFus outperforms state-of-the-art methods for gaze-supervised medical image segmentation.

![](./fig/fig-InPro.png)

# Model Weights
The download links and extraction codes for our model weights are as follows：[Checkpoint](https://pan.baidu.com/s/1cRE9u6sSXicBgcr9r1AgjA?pwd=7777)

# Datasets
1. The MSCMR dataset with mask annotations can be downloaded from [MSCMRseg](https://zmiclab.github.io/zxh/0/mscmrseg19/data.html).
2. The ACDC dataset with mask annotations can be downloaded from [ACDC](https://www.creatis.insa-lyon.fr/Challenge/acdc/).

## Qualitative Results
![1.0](./fig/fig-result.png)

## Requirements
* python 3.8 <br>
* torch 1.12.0<br>
* numpy 1.24.4<br>
* medpy 0.5.1<br>
* nibabel 5.2.1<br>
* pandas 2.0.3<br>
* scikit-image 0.21.0<br>

## Acknowledgement
This repo partially uses code from [CycleMix](https://github.com/BWGZK/CycleMIx).
