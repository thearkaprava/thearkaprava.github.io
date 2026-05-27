---
title: "TimeProVe: Temporally Grounded Reasoning in Long Videos"
permalink: /timeprove/
layout: single
author_profile: false
classes: wide
toc: true
toc_sticky: true
---

<p style="font-size: 1.05em; margin-top: -0.5rem;">
  <strong>TimeProVe</strong> is a cost-efficient hybrid framework for temporally grounded reasoning in long, untrimmed videos. It uses lightweight modules to propose action-grounded answer–evidence hypotheses, and calls an expensive vision-language model only for targeted verification.
</p>

<p style="margin: 1rem 0 1.25rem 0;">
  <a class="btn btn--large" href="/timeprove/TimeProVe.pdf">Paper (PDF)</a>
  <a class="btn btn--large btn--info" href="/timeprove/timeprove_teaser_emnlp26_v2.pdf">Teaser (PDF)</a>
  <a class="btn btn--large btn--inverse" href="/timeprove/main_arch_v2.pdf">Architecture (PDF)</a>
  <a class="btn btn--large btn--inverse" href="/timeprove/otb_overview.pdf">OpenTSUBench (PDF)</a>
</p>

<!-- If you want an author line like mstemba.github.io, fill this in. -->
<!--
<p style="font-size: 1.0em;">
  <em>Arkaprava Sinha</em>, ...<br/>
  UNC Charlotte, ...
</p>
-->

## Abstract

Long Video Question Answering (LVQA) requires identifying sparse, query-relevant evidence within hours-long untrimmed videos. Existing approaches either process videos densely with large vision-language models (VLMs), incurring prohibitive computational cost, or rely on sparse caption-based reasoning, which often misses temporally localized and motion-centric evidence. We introduce TimeProVe, a cost-efficient hybrid framework for temporally grounded reasoning in long videos. TimeProVe first employs lightweight modules to generate action-grounded answer--evidence hypotheses and subsequently invokes an expensive VLM only for targeted verification. The core of our framework lies in the Action-based Candidate Evidence (ACE) module, which converts temporally localized actions into query-conditioned candidate answers and supporting evidence windows through lightweight LLM reasoning. We further introduce OpenTSUBench (OTB), an open-ended benchmark designed to evaluate temporally grounded reasoning in real-world Activities of Daily Living (ADL) scenarios. Experiments show that TimeProVe outperforms the strongest baseline on OTB by 7.3%, while reducing VLM calls by 75% and inference cost by 93%. Furthermore, without explicit temporal grounding training, TimeProVe achieves competitive performance on Charades-STA, and reaches state-of-the-art results when enhanced with grounding VLMs.

## Key idea (high level)

1. Use lightweight modules to propose candidate answers paired with temporally localized evidence windows.
2. Verify only the most promising candidates with a VLM, drastically reducing the number of expensive calls while preserving temporally grounded reasoning.

## TimeProVe framework (overview)

<object data="/timeprove/main_arch_v2.pdf" type="application/pdf" width="100%" height="650px">
  <p>
    PDF preview not supported in your browser.
    <a href="/timeprove/main_arch_v2.pdf">Open the architecture figure (PDF)</a>.
  </p>
</object>

## OpenTSUBench (OTB) overview

<object data="/timeprove/otb_overview.pdf" type="application/pdf" width="100%" height="650px">
  <p>
    PDF preview not supported in your browser.
    <a href="/timeprove/otb_overview.pdf">Open the OTB overview figure (PDF)</a>.
  </p>
</object>

## Teaser

<object data="/timeprove/timeprove_teaser_emnlp26_v2.pdf" type="application/pdf" width="100%" height="650px">
  <p>
    PDF preview not supported in your browser.
    <a href="/timeprove/timeprove_teaser_emnlp26_v2.pdf">Open the teaser (PDF)</a>.
  </p>
</object>

## BibTeX

Replace the fields below once you have the final venue / arXiv ID.

```bibtex
@inproceedings{timeprove2026,
  title     = {TimeProVe: Temporally Grounded Reasoning in Long Videos},
  author    = {Sinha, Arkaprava and others},
  booktitle = {Proceedings of ...},
  year      = {2026}
}
```

