---
title: "<span style='font-variant: small-caps;'>UniEgo</span>: Proxies as Mediators for Unified Egocentric Video Representation Learning"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: ''
date: 2026-05-20
venue: 'Preprint'
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://drive.google.com/file/d/1b1bau_WKn6dPB2BrxCvtBkO3ZIveJKA0/view?usp=share_link'
codeurl: ''
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: 'Wenhao Chi, <span style="font-size: 0.8em;"><strong>Arkaprava Sinha</strong>, Dominick Reilly, Hieu Le, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---


[Paper](https://drive.google.com/file/d/1b1bau_WKn6dPB2BrxCvtBkO3ZIveJKA0/view?usp=share_link)

## Abstract:
Egocentric video understanding is inherently limited by the narrow perspective of wearable cameras: a single viewpoint, a single modality, a single model cannot capture the full richness of human action. We argue that a truly expressive egocen-
tric representation must subsume complementary knowledge across viewpoints, modalities, and foundation model representations, yet remain deployable from egocentric video alone. To this end, we introduce a hierarchical multi-teacher
distillation framework that produces UNIEGO, a unified egocentric encoder trained with 9 teachers spanning ego-exo viewpoints, RGB, depth, and skeleton modalities, and four foundation models. Rather than distilling directly from heterogeneous teachers whose incompatible architectures and feature geometries induce conflicting gradients, our framework interposes a layer of representation-specific Proxy models that translate diverse teacher knowledge into a homogeneous egocentric space. A second distillation stage, Selective Proxy Distillation (SPD), then adaptively selects, for each training sample, the subset of proxies that are both correct and confident, distilling exclusively from reliable supervision and suppressing erroneous signals. SPD is further stabilized by initializing UNIEGO as a learned convex
combination of proxy parameters, placing the unified model in a well-conditioned region of the loss landscape before distillation begins. UNIEGO achieves state-of-the-art performance across three egocentric video understanding tasks - action
recognition, video retrieval, and action segmentation on three challenging ego-exo benchmarks, outperforming naive multi-teacher distillation baselines and demonstrating that structured, proxy-mediated knowledge transfer yields richer and more discriminative egocentric representations.