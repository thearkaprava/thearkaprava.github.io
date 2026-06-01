---
title: "<span style='font-variant: small-caps;'>TimeProVe</span>: Propose, then Verify for Efficient Long Video Temporal Reasoning in Activities of Daily Living"
collection: publications
category: publication
permalink: #/publication/2009-10-01-paper-title-number-1
excerpt: 'TimeProVe uses lightweight modules to propose candidate answers paired with temporally localized evidence windows. Then it verifies only the most promising candidates with a VLM, drastically reducing the number of expensive calls while preserving temporally grounded reasoning.'
date: 2026-06-01
venue: 'Preprint'
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://drive.google.com/file/d/1P6Ha9a0X4w8GVzVWUKOCoH2_Uze94lAq/view?usp=share_link'
codeurl: ''
citation: #'Sinha, Arkaprava, et al. "MS-Temba: Multi-Scale Temporal Mamba for Efficient Temporal Action Detection." arXiv preprint arXiv:2501.06138 (2025).'
authors: '<span style="font-size: 0.8em;"><strong>Arkaprava Sinha</strong>, Dominick Reilly, Siddharth Krishnan, Hieu Le, Srijan Das</span>'
image: #'image-alignment-300x200.jpg'
---


[Paper](https://drive.google.com/file/d/1P6Ha9a0X4w8GVzVWUKOCoH2_Uze94lAq/view?usp=share_link), [Website](https://thearkaprava.github.io/timeprove/)

## Abstract:
Long Video Question Answering (LVQA) requires identifying sparse, query-relevant evidence within hours-long untrimmed videos. Existing approaches either process videos densely with large vision-language models (VLMs), incurring prohibitive computational cost, or rely on sparse caption-based reasoning, which often misses temporally localized and motion-centric evidence. We introduce TimeProVe, a cost-efficient hybrid framework for temporally grounded reasoning in long videos. TimeProVe first employs lightweight modules to generate action-grounded answer--evidence hypotheses and subsequently invokes an expensive VLM only for targeted verification. The core of our framework lies in the Action-based Candidate Evidence (ACE) module, which converts temporally localized actions into query-conditioned candidate answers and supporting evidence windows through lightweight LLM reasoning. We further introduce OpenTSUBench (otb), an open-ended benchmark designed to evaluate temporally grounded reasoning in real-world Activities of Daily Living (ADL) scenarios. Experiments show that TimeProVe outperforms the strongest baseline on otb by 7.3%, while reducing VLM calls by 75% and inference cost by 93%. Furthermore, without explicit temporal grounding training, TimeProVe achieves competitive performance on Charades-STA, and reaches state-of-the-art results when enhanced with grounding VLMs.