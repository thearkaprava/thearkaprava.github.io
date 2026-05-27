---
title: "TimeProVe"
permalink: /timeprove/
layout: timeprove
---

<div class="timeprove-hero">
  <h1 class="timeprove-title">
    <span class="tp-sc">TimeProVe</span>: Propose, then Verify for Efficient Long Video Temporal Reasoning in Activities of Daily Living
  </h1>
  <p class="timeprove-subtitle">
    A cost-efficient framework for temporally grounded reasoning in long, untrimmed videos.
  </p>

  <div class="column has-text-centered">
    <div class="publication-links">
      <span class="link-block">
        <a href="#" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="ai ai-arxiv"></i>
          </span>
          <span>Paper</span>
        </a>
      </span>

      <span class="link-block">
        <a href="#" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="fab fa-github"></i>
          </span>
          <span>Code</span>
        </a>
      </span>

      <span class="link-block">
        <a href="#" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span>🤗 Data</span>
        </a>
      </span>
    </div>
  </div>
</div>

<div class="abstract-grid">
  <div>
    <h2>Abstract</h2>

Long Video Question Answering (LVQA) requires identifying sparse, query-relevant evidence within hours-long untrimmed videos. Existing approaches either process videos densely with large vision-language models (VLMs), incurring prohibitive computational cost, or rely on sparse caption-based reasoning, which often misses temporally localized and motion-centric evidence. We introduce <span class="tp-sc">TimeProVe</span>, a cost-efficient hybrid framework for temporally grounded reasoning in long videos. <span class="tp-sc">TimeProVe</span> first employs lightweight modules to generate action-grounded answer--evidence hypotheses and subsequently invokes an expensive VLM only for targeted verification. The core of our framework lies in the Action-based Candidate Evidence (ACE) module, which converts temporally localized actions into query-conditioned candidate answers and supporting evidence windows through lightweight LLM reasoning. We further introduce <span class="tp-sc">OpenTSUBench</span> (<span class="tp-sc">otb</span>), an open-ended benchmark designed to evaluate temporally grounded reasoning in real-world Activities of Daily Living (ADL) scenarios. Experiments show that <span class="tp-sc">TimeProVe</span> outperforms the strongest baseline on <span class="tp-sc">otb</span> by 7.3%, while reducing VLM calls by 75% and inference cost by 93%. Furthermore, without explicit temporal grounding training, <span class="tp-sc">TimeProVe</span> achieves competitive performance on Charades-STA, and reaches state-of-the-art results when enhanced with grounding VLMs.
  </div>

  <div class="teaser-panel">
    <img src="{{ base_path }}/timeprove/teaset.png" alt="TimeProVe teaser" />
    <p class="teaser-caption"><span class="tp-sc">TimeProVe</span> reduces long-video LVQA cost by proposing query-relevant evidence locally before VLM verification. Instead of processing the full video, it sends only short targeted clips to the cloud VLM.</p>
  </div>
</div>

## TL;DR

Use lightweight modules to propose candidate answers paired with temporally localized evidence windows. <br>
Verify only the most promising candidates with a VLM, drastically reducing the number of expensive calls while preserving temporally grounded reasoning.

## <span class="tp-sc">TimeProVe</span> framework

![TimeProVe framework overview]({{ base_path }}/timeprove/main_arch.png)
<p class="figure-caption">ACE first builds an action timeline from the full video, then uses query-conditioned proposal generation and reranking to produce candidate answer-evidence hypotheses. A temporal verifier sends only the top short RGB clip to a VLM for confirmation, iterating to the next candidate only when needed, which preserves temporal grounding while substantially reducing expensive full-video inference.</p>

## <span class="tp-sc">OpenTSUBench</span> (<span class="tp-sc">otb</span>)

![OpenTSUBench (OTB) overview]({{ base_path }}/timeprove/otb_benchmark.png)
<p class="figure-caption"><span class="tp-sc">OpenTSUBench</span> is an open-ended, temporally grounded LVQA benchmark for real-world untrimmed ADL videos, where each question is paired with supporting temporal evidence. It includes diverse strata such as temporal positioning, long-horizon sparse evidence, object-centric actions, concurrent activities, and state transitions to evaluate both answer correctness and evidence localization.</p>

<!-- ## BibTeX
```bibtex
@inproceedings{timeprove2026,
  title     = {{\textsc{TimeProVe}}: Temporally Grounded Reasoning in Long Videos},
  author    = {Sinha, Arkaprava and others},
  booktitle = {},
  year      = {2026}
}
``` -->

