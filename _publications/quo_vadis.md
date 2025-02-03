---
title: "Quo Vadis, Video Understanding with Vision-Language Foundation Models?"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'This study benchmarks Vision-Language Models (VLMs & VLLMs) on five ADL video tasks across 11 datasets, revealing their struggles with fine-grained action understanding. Despite their web-scale success, these models fall short on real-world, densely labeled, and long-video challenges.'
date: 2024-12-10
venue: NeurIPSW 
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://hal.science/hal-04893035/document'
codeurl: #'https://github.com/ADL-X/LLAVIDAL'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;">Mahmoud Ali, Di Yang, <strong>Arkaprava Sinha</strong>, Dominick Reilly, Srijan Das,
Gianpiero Francesca, Francois Bremond</span>'
image: #'image-alignment-300x200.jpg'
---

[Paper](https://hal.science/hal-04893035/document)

## Abstract:
Vision-Language foundation models, including vision-language models (VLMs) and vision-large language models (VLLMs), have been evolving rapidly and have shown good performance on different downstream video understanding tasks, especially on web datasets. However, it is still an open question how much these VLMs and VLLMs perform in more challenging scenarios like Activities of Daily Living (ADL). To answer this, we provide a comprehensive study of VLMs and VLLMs by comparing their zero-shot transfer ability to five downstream tasks including action classification, video retrieval, video description, action forecasting, and frame-wise action segmentation. Extensive experiments are conducted on eleven real-world, human-centric video understanding datasets (e.g., Toyota Smarthome, Penn Action, UAV-Human, EgoExo4D, TSU, Charades) to study these tasks with our insights into the strengths and limitations of these models in zero-shot settings. Moreover, we provide in-deep analysis to find the best setting to improve the model performance in zero-shot action classification tasks. Based on our experiments, we find that these models are still far away from satisfactory performance in all evaluated tasks, particularly in densely labeled and long video datasets.