---
layout: minimal
title: ""
permalink: /
description: "Arkaprava Sinha — PhD researcher in Computer Vision, working on long video understanding and multimodal vision-language models at UNC Charlotte."
redirect_from:
  - /about/
  - /about.html
---

<div class="intro">
  <div class="intro-text">
    <h1>Arkaprava Sinha</h1>
    <p class="role">PhD Student, Computer Vision · UNC Charlotte</p>
    <p class="loc"><i class="fas fa-location-dot"></i>Charlotte, North Carolina</p>
    <p class="contact">
      <i class="fas fa-envelope"></i><a href="mailto:asinha13@charlotte.edu">Email</a><span class="sep">/</span>
      <i class="ai ai-google-scholar"></i><a href="https://scholar.google.com/citations?user=igxv5JYAAAAJ&hl=en">Scholar</a><span class="sep">/</span>
      <i class="fab fa-github"></i><a href="https://github.com/thearkaprava">GitHub</a><span class="sep">/</span>
      <i class="fab fa-linkedin"></i><a href="https://www.linkedin.com/in/arkaprava-sinha">LinkedIn</a><span class="sep">/</span>
      <i class="fas fa-file-pdf"></i><a href="{{ base_path }}/files/Arkaprava_Sinha_CV.pdf">CV</a>
    </p>
  </div>
  <img class="photo" src="{{ base_path }}/images/profile_AS.jpeg" alt="Arkaprava Sinha" width="500" height="667" fetchpriority="high">
</div>

I am a Graduate Research Assistant pursuing a Ph.D. in Computer Science at the [University of North Carolina at Charlotte](https://cci.charlotte.edu), advised by [Prof. Srijan Das](https://srijandas07.github.io). My research lies at the intersection of multimodal vision-language models, long-context video understanding, temporal modeling, and agentic systems, with a focus on building scalable and reliable algorithms for long video understanding.

Prior to my Ph.D., I worked as a Data Scientist, contributing to projects in computer vision, natural language processing, and large-scale machine learning across industry and research settings.

## Research

<p class="lead">I build efficient multimodal AI systems that can understand and reason over long, untrimmed videos of everyday human activity.</p>

My research focuses on building efficient multimodal AI systems for long-horizon video understanding, egocentric perception, and visual reasoning. I design scalable temporal architectures and representation-learning methods that help models reason over long, untrimmed videos, align video with language, motion, and structured visual cues, and operate efficiently in real-world settings.

I am particularly interested in *agentic video understanding*, where systems actively search for relevant evidence, reason over temporal context, and verify answers using multimodal foundation models instead of exhaustively processing entire videos. Broadly, my work connects long video understanding, vision-language models, multimodal LLMs, diffusion-based generation, and embodied AI — with applications in robotics, AR/VR, intelligent assistants, assistive technology, and safety-critical video analytics.

## News

<div class="news">
  <div class="news-item"><div class="date">Feb 2026</div><div class="what"><span class="sc">MS-Temba</span> accepted to CVPR 2026.</div></div>
  <div class="news-item"><div class="date">Feb 2025</div><div class="what"><span class="sc">LLAVIDAL</span> accepted to CVPR 2025.</div></div>
  <div class="news-item"><div class="date">Dec 2024</div><div class="what"><span class="sc">SKI Models</span> accepted to AAAI 2025.</div></div>
  <div class="news-item"><div class="date">Oct 2024</div><div class="what">2 papers accepted to NeurIPS 2024 workshops; an early version of <span class="sc">LLAVIDAL</span> presented at the NeurIPS 2024 Workshop on Video-Language Models and Multimodal Algorithmic Reasoning.</div></div>
</div>

## Selected Publications

<div class="pub">
  <div class="thumb"><video src="{{ base_path }}/timeprove/assets/TimeProVe_demo_video_teaser.mp4" autoplay loop muted playsinline preload="metadata" onerror="this.closest('.thumb').style.display='none'"></video></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/abs/2606.20561"><span class="sc">TimeProVe</span>: Propose, then Verify for Efficient Long Video Temporal Reasoning in Activities of Daily Living</a></div>
    <div class="authors"><span class="me">Arkaprava Sinha</span>, Dominick Reilly, Siddharth Krishnan, Hieu Le, Srijan Das</div>
    <div class="venue">Preprint, 2026</div>
    <div class="desc">A hybrid long-video reasoning framework that proposes action-grounded hypotheses efficiently, then verifies only sparse RGB evidence with an expensive VLM.</div>
    <div class="links"><a href="https://arxiv.org/abs/2606.20561">Paper</a> / <a href="https://github.com/thearkaprava/TimeProVe">Code</a> / <a href="https://thearkaprava.github.io/timeprove/">Website</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><img src="{{ base_path }}/images/papers/uniego.png" alt="UniEgo" loading="lazy" onerror="this.closest('.thumb').style.display='none'"></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/abs/2606.20559"><span class="sc">UniEgo</span>: Proxies as Mediators for Unified Egocentric Video Representation Learning</a></div>
    <div class="authors">Wenhao Chi, <span class="me">Arkaprava Sinha</span>, Dominick Reilly, Hieu Le, Srijan Das</div>
    <div class="venue">Preprint, 2026</div>
    <div class="desc">A unified egocentric encoder trained via hierarchical distillation across ego-exo viewpoints, modalities, and foundation models, using representation-specific proxies as mediators.</div>
    <div class="links"><a href="https://arxiv.org/abs/2606.20559">Paper</a> / <a href="https://github.com/Wenhao-Chi/UNIEGO">Code</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><video src="{{ base_path }}/images/papers/ms-temba-web.mp4" autoplay loop muted playsinline preload="metadata" onerror="this.closest('.thumb').style.display='none'"></video></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/abs/2501.06138">MS-Temba: Multi-Scale Temporal Mamba for Understanding Long Untrimmed Videos</a></div>
    <div class="authors"><span class="me">Arkaprava Sinha</span>, Monish Soundar Raj, Pu Wang, Ahmed Helmy, Hieu Le, Srijan Das</div>
    <div class="venue">IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026</div>
    <div class="desc">The first Mamba-based architecture for temporal action detection in long untrimmed videos — only 17M parameters, trainable on an NVIDIA Jetson Nano.</div>
    <div class="links"><a href="https://arxiv.org/abs/2501.06138">Paper</a> / <a href="https://github.com/thearkaprava/MS-Temba">Code</a> / <a href="https://mstemba.github.io">Website</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><img src="{{ base_path }}/images/papers/diffswap.png" alt="DiffSwap++" loading="lazy" onerror="this.closest('.thumb').style.display='none'"></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/pdf/2511.05575">DiffSwap++: 3D Latent-Controlled Diffusion for Identity-Preserving Face Swapping</a></div>
    <div class="authors">Weston Bondurant, <span class="me">Arkaprava Sinha</span>, Hieu Le, Srijan Das, Stephanie Schuckers</div>
    <div class="venue">IEEE/IAPR International Joint Conference on Biometrics (IJCB), 2026</div>
    <div class="desc">3D latent-controlled diffusion for identity-preserving face swapping.</div>
    <div class="links"><a href="https://arxiv.org/pdf/2511.05575">Paper</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><img src="{{ base_path }}/images/papers/llavidal.png" alt="LLAVIDAL" loading="lazy" onerror="this.closest('.thumb').style.display='none'"></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/abs/2406.09390">LLAVIDAL: A Large Language Vision Model for Daily Activities of Living</a></div>
    <div class="authors">Dominick Reilly, Rajatsubhra Chakraborty, <span class="me">Arkaprava Sinha</span>, Manish Kumar Govind, Pu Wang, Francois Bremond, Le Xue, Srijan Das</div>
    <div class="venue">IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025</div>
    <div class="desc">A large language-vision model that incorporates 3D poses and object trajectories to understand the spatiotemporal relationships within daily living activities.</div>
    <div class="links"><a href="https://arxiv.org/abs/2406.09390">Paper</a> / <a href="https://github.com/ADL-X/LLAVIDAL">Code</a> / <a href="https://adl-x.github.io">Website</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><img src="{{ base_path }}/images/papers/ski-models.jpg" alt="SKI Models" loading="lazy" onerror="this.closest('.thumb').style.display='none'"></div>
  <div class="body">
    <div class="title"><a href="https://arxiv.org/abs/2502.03459">SKI Models: Skeleton Induced Vision-Language Embeddings for Understanding Activities of Daily Living</a></div>
    <div class="authors"><span class="me">Arkaprava Sinha</span>, Dominick Reilly, Francois Bremond, Pu Wang, Srijan Das</div>
    <div class="venue">39th Annual AAAI Conference on Artificial Intelligence (AAAI), 2025</div>
    <div class="desc">Introduces 3D skeletons into the vision-language embedding space to enable effective zero-shot learning for activities of daily living.</div>
    <div class="links"><a href="https://arxiv.org/abs/2502.03459">Paper</a> / <a href="https://github.com/thearkaprava/SKI-Models">Code</a></div>
  </div>
</div>

<div class="pub">
  <div class="thumb"><img src="{{ base_path }}/images/papers/quo-vadis.png" alt="Quo Vadis" loading="lazy" onerror="this.closest('.thumb').style.display='none'"></div>
  <div class="body">
    <div class="title"><a href="https://hal.science/hal-04893035/document">Quo Vadis, Video Understanding with Vision-Language Foundation Models?</a></div>
    <div class="authors">Mahmoud Ali, Di Yang, <span class="me">Arkaprava Sinha</span>, Dominick Reilly, Srijan Das, Gianpiero Francesca, Francois Bremond</div>
    <div class="venue">NeurIPS Workshop on Video-Language Models, 2024</div>
    <div class="desc">A study of where video understanding stands with vision-language foundation models, and where it should go next.</div>
    <div class="links"><a href="https://hal.science/hal-04893035/document">Paper</a></div>
  </div>
</div>

<p style="font-size:.92rem;color:var(--muted);margin-top:1.4rem;">See the <a href="{{ base_path }}/publications/">full list of publications</a>.</p>
