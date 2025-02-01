---
title: "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'Multi-scale Temporal Mamba adapts Mamba for action detection in long untrimmed videos by introducing Temporal Mamba (Temba) Blocks with dilated temporal modeling and a Temporal Mamba Fuser for multi-scale feature aggregation. It outperforms SOTA methods on long videos while being significantly more efficient.'
date: 2025-01-12
venue: 'preprint'
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2501.06138'
codeurl: 'https://github.com/thearkaprava/MS-Temba'
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;"><strong>Arkaprava Sinha</strong>, Monish Soundar Raj, Pu Wang, Ahmed Helmy, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---


[Paper](https://arxiv.org/abs/2501.06138), [Code](https://github.com/thearkaprava/MS-Temba)

## Abstract:
Action detection in real-world scenarios is particularly challenging due to densely distributed actions in hour-long untrimmed videos. It requires modeling both short- and long-term temporal relationships while handling significant intra-class temporal variations. Previous state-of-the-art (SOTA) Transformer-based architectures, though effective, are impractical for real-world deployment due to their high parameter count, GPU memory usage, and limited throughput, making them unsuitable for very long videos.

In this work, we innovatively adapt the Mamba architecture for action detection and propose **Multi-scale Temporal Mamba (MS-Temba)**, comprising two key components: *Temporal Mamba (Temba) Blocks* and the *Temporal Mamba Fuser*. Temba Blocks include the Temporal Local Module (TLM) for short-range temporal modeling and the Dilated Temporal SSM (DTS) for long-range dependencies. By introducing dilations, a novel concept for Mamba, TLM and DTS capture local and global features at multiple scales. The Temba Fuser aggregates these scale-specific features using Mamba to learn comprehensive multi-scale representations of untrimmed videos.

MS-Temba is validated on three public datasets, outperforming SOTA methods on long videos and matching prior methods on short videos while using only one-eighth of the parameters. 