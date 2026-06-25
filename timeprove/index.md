---
title: "TimeProVe"
permalink: /timeprove/
layout: timeprove
---

<section class="tp-section">
  <div class="tp-section-inner">

<div class="timeprove-hero">
  <h1 class="timeprove-title">
    <span class="tp-sc">TimeProVe</span>: Propose, then Verify for Efficient Long Video Temporal Reasoning in Activities of Daily Living
  </h1>
  <p class="timeprove-subtitle">
    A cost-efficient framework for temporally grounded reasoning in long, untrimmed videos.
  </p>

  <div class="column has-text-centered">
    <div class="is-size-5 publication-authors" style="margin-bottom: 0.75rem; text-align: center;">
      <span class="author-block">
        <a href="https://thearkaprava.github.io" target="_blank">Arkaprava Sinha</a>,
      </span>
      <span class="author-block">
        <a href="https://dominickrei.github.io/" target="_blank">Dominick Reilly</a>,
      </span>
      <span class="author-block">
        <a href="https://webpages.charlotte.edu/skrish21/" target="_blank">Siddharth Krishnan</a>,
      </span>
      <span class="author-block">
        <a href="https://hieulem.github.io" target="_blank">Hieu Le</a>,
      </span>
      <span class="author-block">
        <a href="https://srijandas07.github.io" target="_blank">Srijan Das</a>
      </span>
    </div>
    <div class="is-size-5 publication-authors" style="margin-bottom: 1rem; text-align: center;">
      <span class="author-block">University of North Carolina at Charlotte</span>
    </div>

    <div class="publication-links">
      <span class="link-block">
        <a href="https://arxiv.org/abs/2606.20561" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="ai ai-arxiv"></i>
          </span>
          <span>Paper</span>
        </a>
      </span>

      <span class="link-block">
        <a href="https://github.com/thearkaprava/TimeProVe" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="fab fa-github"></i>
          </span>
          <span>Code</span>
        </a>
      </span>

      <span class="link-block">
        <a href="https://huggingface.co/datasets/thearkaprava/OpenTSUBench/tree/main" target="_blank" class="external-link button is-normal is-rounded is-dark">
          <span>🤗 Data</span>
        </a>
      </span>
    </div>
  </div>
</div>

  </div>
</section>

<section class="tp-section">
  <div class="tp-section-inner">

<div class="abstract-grid">
  <div>
    <h2>Abstract</h2>
    <p>Long Video Question Answering (LVQA) requires identifying sparse, query-relevant evidence within hours-long untrimmed videos. Existing approaches either process videos densely with large vision-language models (VLMs), incurring prohibitive computational cost, or rely on sparse caption-based reasoning, which often misses temporally localized and motion-centric evidence. We introduce <span class="tp-sc">TimeProVe</span>, a cost-efficient hybrid framework for temporally grounded reasoning in long videos. <span class="tp-sc">TimeProVe</span> first employs lightweight modules to generate action-grounded answer--evidence hypotheses and subsequently invokes an expensive VLM only for targeted verification. The core of our framework lies in the Action-based Candidate Evidence (ACE) module, which converts temporally localized actions into query-conditioned candidate answers and supporting evidence windows through lightweight LLM reasoning. We further introduce <span class="tp-sc">OpenTSUBench</span> (<span class="tp-sc">otb</span>), an open-ended benchmark designed to evaluate temporally grounded reasoning in real-world Activities of Daily Living (ADL) scenarios. Experiments show that <span class="tp-sc">TimeProVe</span> outperforms the strongest baseline on <span class="tp-sc">otb</span> by 7.3%, while reducing VLM calls by 75% and inference cost by 93%. Furthermore, without explicit temporal grounding training, <span class="tp-sc">TimeProVe</span> achieves competitive performance on Charades-STA, and reaches state-of-the-art results when enhanced with grounding VLMs.</p>
  </div>

  <div class="teaser-panel">
    <img src="{{ base_path }}/timeprove/teaset.jpg" alt="TimeProVe teaser" width="1200" height="1157" loading="eager" />
    <p class="teaser-caption"><span class="tp-sc">TimeProVe</span> reduces long-video LVQA cost by proposing query-relevant evidence locally before VLM verification. Instead of processing the full video, it sends only short targeted clips to the cloud VLM.</p>
  </div>
</div>

<div class="tp-tldr">
  <h2>TL;DR</h2>
  <p>Use lightweight modules to propose candidate answers paired with temporally localized evidence windows.<br>
  Verify only the most promising candidates with a VLM, drastically reducing the number of expensive calls while preserving temporally grounded reasoning.</p>
</div>

  </div>
</section>

<section class="tp-section">
  <div class="tp-section-inner">

<h2><span class="tp-sc">TimeProVe</span> framework</h2>

<img src="{{ base_path }}/timeprove/main_arch.jpg" alt="TimeProVe framework overview" width="1400" height="682" loading="lazy" />
<p class="figure-caption">ACE first builds an action timeline from the full video, then uses query-conditioned proposal generation and reranking to produce candidate answer-evidence hypotheses. A temporal verifier sends only the top short RGB clip to a VLM for confirmation, iterating to the next candidate only when needed, which preserves temporal grounding while substantially reducing expensive full-video inference.</p>

  </div>
</section>

<section class="tp-section">
  <div class="tp-section-inner">

<h2><span class="tp-sc">OpenTSUBench</span> (<span class="tp-sc">otb</span>)</h2>

<img src="{{ base_path }}/timeprove/otb_benchmark.jpg" alt="OpenTSUBench (OTB) overview" width="1400" height="675" loading="lazy" />
<p class="figure-caption"><span class="tp-sc">OpenTSUBench</span> is an open-ended, temporally grounded LVQA benchmark for real-world untrimmed ADL videos, where each question is paired with supporting temporal evidence. It includes diverse strata such as temporal positioning, long-horizon sparse evidence, object-centric actions, concurrent activities, and state transitions to evaluate both answer correctness and evidence localization.</p>

  </div>
</section>

<section class="tp-section">
  <div class="tp-section-inner">

<h2>Qualitative Examples</h2>

<div class="demo-video-grid">
  <div class="demo-video-panel demo-video-panel--square">
    <video class="timeprove-demo-video" width="1000" height="1000" autoplay loop muted playsinline preload="auto">
      <source src="{{ base_path }}/timeprove/assets/TimeProVe_demo_P02T01C06.mp4" type="video/mp4">
    </video>
  </div>
  <div class="demo-video-panel">
    <video class="timeprove-demo-video" width="760" height="840" autoplay loop muted playsinline preload="auto">
      <source src="{{ base_path }}/timeprove/assets/TimeProVe_demo_P02T04C04_c092.mp4" type="video/mp4">
    </video>
  </div>
  <div class="demo-video-panel">
    <video class="timeprove-demo-video" width="760" height="814" autoplay loop muted playsinline preload="auto">
      <source src="{{ base_path }}/timeprove/assets/TimeProVe_demo_P02T07C04_c138.mp4" type="video/mp4">
    </video>
  </div>
  <div class="demo-video-panel">
    <video class="timeprove-demo-video" width="760" height="814" autoplay loop muted playsinline preload="auto">
      <source src="{{ base_path }}/timeprove/assets/TimeProVe_demo_P10T02C05_c136.mp4" type="video/mp4">
    </video>
  </div>
</div>
<p class="figure-caption"><span class="tp-sc">TimeProVe</span> localizes sparse temporal evidence from a long ADL video and verifies query-relevant clips using a VLM, avoiding full-video processing.</p>

  </div>
</section>

<section class="tp-section tp-section--plain">
  <div class="tp-section-inner">

<h2>BibTeX</h2>

<div class="bibtex-block">
  <button type="button" class="bibtex-copy-btn" data-copy-target="timeprove-bibtex" aria-label="Copy BibTeX to clipboard">
    <i class="fa-regular fa-copy"></i> Copy
  </button>
  <pre class="bibtex-code"><code id="timeprove-bibtex">@misc{sinha2026timeprove,
      title={TimeProVe: Propose, then Verify for Efficient Long Video Temporal Reasoning in Activities of Daily Living},
      author={Arkaprava Sinha and Dominick Reilly and Siddharth Krishnan and Hieu Le and Srijan Das},
      year={2026},
      eprint={2606.20561},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2606.20561},
}</code></pre>
</div>

  </div>
</section>
