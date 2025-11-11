---
title: "DiffSwap++: 3D Latent-Controlled Diffusion for Identity-Preserving Face Swapping"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: '3D Guided Diffusion for Face Swapping'
date: 2025-11-10
venue: preprint
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2511.05575'
codeurl: #'https://github.com/ADL-X/LLAVIDAL'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;">Weston Bondurant, <strong>Arkaprava Sinha</strong>, Hieu Le, Srijan Das, Stephanie Schuckers</span>'
image: #'image-alignment-300x200.jpg'
---

[Paper](https://arxiv.org/pdf/2511.05575)

## Abstract:
 Diffusion-based approaches have recently achieved strong results in face swapping, offering improved visual quality over traditional GAN-based methods. However, even state-of-the-art models often suffer from fine-grained artifacts and poor identity preservation. A key limitation of existing approaches is their failure to meaningfully leverage 3D facial structure, which is crucial for disentangling identity from pose and expression. In this work, we propose DiffSwap++, a novel diffusionbased pipeline that incorporates 3D facial latent features while generating face swaps. By guiding the generation process with 3D-aware representations, our method enhances geometric consistency and improves the disentanglement of facial identity
from appearance attributes. We further design a diffusion architecture that conditions the denoising process on both identity
embeddings and facial landmarks, enabling high-fidelity and identity-preserving face swaps. Extensive experiments on three public datasets: CelebA, FFHQ, and CelebV-Text demonstrate that DiffSwap++ outperforms prior methods in preserving source identity while maintaining comparable target pose and expression. Additionally, we introduce a biometric-style evaluation and conduct a user study to further validate the realism and effectiveness of our approach.