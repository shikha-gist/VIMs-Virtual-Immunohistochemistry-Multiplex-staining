# Virtual Immunohistochemistry Multiplex Staining (VIMs) Model

This repository contains the code for the paper *"VIMs: Virtual Immunohistochemistry Multiplex staining via
Text-to-Stain Diffusion Trained on Uniplex Stains"*, which introduces a Virtual Immunohistochemistry Multiplex staining (VIMs) model designed to generate multiple immunohistochemistry (IHC) stains from a single hematoxylin and eosin (H&E) stained tissue section.\

![image](https://github.com/user-attachments/assets/c68552ed-b018-426a-af50-9c3d78ee428f)


## Overview

IHC stains are crucial in pathology practice for resolving complex diagnostic questions and guiding patient treatment decisions. Commercial laboratories offer a wide array of up to 400 different antibody-based IHC stains, but small biopsies often lack sufficient tissue for multiple stains while preserving material for subsequent molecular testing. This highlights the need for virtual IHC staining.

**VIMs** is the first model to address this need, leveraging a large vision-language single-step diffusion model for virtual IHC multiplexing through text prompts for each IHC marker. Key features of VIMs include:

- **Training Data**: VIMs is trained on uniplex paired H&E and IHC images, employing an adversarial training module.
- **Efficiency**: The model utilizes a pre-trained large latent diffusion model fine-tuned with small, trainable weights through the Low-Rank Adapter (LoRA) approach.
- **Performance**: Experiments on nuclear and cytoplasmic IHC markers demonstrate that VIMs outperforms the base diffusion model and achieves performance comparable to Pix2Pix, a standard generative model for paired image translation.
- **Evaluation**: Multiple evaluation methods, including assessments by two pathologists, are used to determine the performance of VIMs. Experiments with different prompts highlight the impact of text conditioning.

This work represents the first attempt to accelerate histopathology research by generating multiple IHC stains from a single H&E input using a single model trained solely on uniplex data. This approach relaxes the traditional need for multiplex training sets, significantly broadening the applicability and accessibility of virtual IHC staining techniques.

## Code Status

The code for VIMs will be updated soon. Please check back later for the full implementation.

## Paper

For more details, please refer to our paper:  
[https://arxiv.org/pdf/2407.19113](#)

## Citation

If you find this work useful in your research, please consider citing our paper:

```bibtex
@article{VIMs,
  title={VIMs: Virtual Immunohistochemistry Multiplex staining via Text-to-Stain Diffusion Trained on Uniplex Stains},
  author={Shikha Dubey, Yosep Chong, Beatrice Knudsen, and Shireen Y. Elhabian},
  journal={Medical Image Computing and Computer-Assisted Intervention-Workshop (MICCAI-W) (MLMI)![image]
},
  year={2024},
  url={https://arxiv.org/pdf/2407.19113}
}



This repository will be updated soon !
