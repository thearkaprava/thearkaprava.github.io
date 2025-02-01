---
title: "SKI Models: Skeleton Induced Vision-Language Embeddings for Understanding Activities of Daily Living"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'SKI models integrate 3D skeletons into vision-language models using SkeletonCLIP, enabling improved generalization to unseen actions in ADL videos. They enhance robustness by not requiring skeleton data during inference and show effectiveness in zero-shot action recognition and video captioning.'
date: 2025-02-4
venue: AAAI
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2501.06138'
codeurl: 'https://github.com/thearkaprava/SKI-Models'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;"><strong>Arkaprava Sinha</strong>, Dominick Reilly, Francois Bremond, Pu Wang, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---

[Paper](https://arxiv.org/abs/2501.06138), [Code](https://github.com/thearkaprava/SKI-Models)

## Abstract:
The introduction of vision-language models like CLIP has enabled the development of foundational video models capable of generalizing to unseen videos and human actions. However, these models are typically trained on web videos, which often fail to capture the challenges present in Activities of Daily Living (ADL) videos. Existing works address ADL-specific challenges, such as *similar appearances*, *subtle motion patterns*, and *multiple viewpoints*, by combining 3D skeletons and RGB videos. However, these approaches are not integrated with language, limiting their ability to generalize to unseen action classes.
In this paper, we introduce **SKI models**, which integrate 3D skeletons into the vision-language embedding space. SKI models leverage a skeleton-language model, **SkeletonCLIP**, to infuse skeleton information into Vision Language Models (VLMs) and Large Vision Language Models (LVLMs) through collaborative training. Notably, SKI models do not require skeleton data during inference, enhancing their robustness for real-world applications. The effectiveness of SKI models is validated on three popular ADL datasets for zero-shot action recognition and video caption generation tasks.