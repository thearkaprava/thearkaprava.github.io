---
title: "LLAVIDAL: A Large Language Vision Model for Daily Activities of Living"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'LLAVIDAL, a Large Language Vision Model, incorporates 3D poses and relevant object trajectories to understand the intricate spatiotemporal relationships within ADLs.'
date: 2025-02-26
venue: CVPR 
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2406.09390'
codeurl: 'https://github.com/ADL-X/LLAVIDAL'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;">Dominick Reilly, Rajatsubhra Chakraborty, <strong>Arkaprava Sinha</strong>, Manish Kumar Govind, Pu Wang, Francois Bremond, Le Xue, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---

[Paper](https://arxiv.org/abs/2406.09390), [Code](https://github.com/ADL-X/LLAVIDAL), [Website](https://adl-x.github.io/)

## Abstract:
Current Large Language Vision Models (LLVMs) trained on web videos perform well in general video understanding but struggle with fine-grained details, complex human-object interactions (HOI), and view-invariant representation learning essential for Activities of Daily Living (ADL). This limitation stems from a lack of specialized ADL video instruction-tuning datasets and insufficient modality integration to capture discriminative action representations. To address this, we propose a semi-automated framework for curating ADL datasets, creating **ADL-X**, a multiview, multimodal RGBS instruction-tuning dataset. Additionally, we introduce **LLAVIDAL**, an LLVM integrating videos, 3D skeletons, and HOIs to model ADL's complex spatiotemporal relationships. For training LLAVIDAL a simple joint alignment of all modalities yields suboptimal results; thus, we propose a Multimodal Progressive (**MMPro**) training strategy, incorporating modalities in stages following a curriculum. We also establish ADL MCQ and video description benchmarks to assess LLVM performance in ADL tasks. Trained on ADL-X, LLAVIDAL achieves state-of-the-art performance across ADL benchmarks. Code and data is publicly available at [https://adl-x.github.io/](https://adl-x.github.io/).