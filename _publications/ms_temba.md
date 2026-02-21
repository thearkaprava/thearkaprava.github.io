---
title: "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'Multi-scale Temporal Mamba adapts Mamba for action detection in long untrimmed videos by introducing Temporal Mamba (Temba) Blocks with dilated temporal modeling and a Temporal Mamba Fuser for multi-scale feature aggregation. It outperforms SOTA methods on long videos while being significantly more efficient.'
date: 2026-02-20
venue: 'CVPR'
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2501.06138'
codeurl: 'https://github.com/thearkaprava/MS-Temba'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;"><strong>Arkaprava Sinha</strong>, Monish Soundar Raj, Pu Wang, Ahmed Helmy, Hieu Le, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---


[Paper](https://arxiv.org/abs/2501.06138), [Code](https://github.com/thearkaprava/MS-Temba), [Website](https://mstemba.github.io)

## Abstract:
Temporal Action Detection (TAD) in untrimmed videos poses significant challenges, particularly for Activities of Daily Living (ADL) requiring models to (1) process long-duration videos, (2) capture temporal variations in actions, and (3) simultaneously detect dense overlapping actions. Existing CNN and Transformer-based approaches, struggle to jointly capture fine-grained detail and long-range structure at scale. State-space Model (SSM) based Mamba offers powerful long-range modeling, but naive application to TAD collapses fine-grained temporal structure and fails to account for the challenges inherent to TAD. To this end, we propose Multi-Scale Temporal Mamba (MS-Temba), which extends Mamba to TAD with newly introduced dilated SSMs. Each Temba block, comprising dilated SSMs coupled with our proposed additional losses, enables the learning of discriminative representations across temporal scales. A lightweight Multi-scale Mamba Fuser then unifies these multi-scale features via SSM-based aggregation, yielding precise action-boundary localization. 

With only 17M parameters, MS-Temba achieves state-of-the-art performance on densely labeled ADL benchmarks TSU & Charades, and further generalizes to long-form video summarization, setting new state-of-the-art results on TVSum & SumMe.