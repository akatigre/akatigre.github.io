---
layout: research
permalink: /
title: "Yoonjeon Kim"
---

<!-- ── HERO ─────────────────────────────────────────────────── -->
<section class="r-hero r-fade">
  <div class="r-photo-wrap">
    <img class="r-photo" src="/assets/images/yjk_profile.png" alt="Yoonjeon Kim">
  </div>
  <div class="r-hero-text">
    <h1 class="r-name">Yoonjeon Kim</h1>
    <p class="r-tagline">
      Ph.D. candidate at <a href="https://mli.kaist.ac.kr/">KAIST ML &amp; Intelligence Lab</a>,
      advised by <a href="https://sites.google.com/site/yangeh/">Prof. Eunho Yang</a>.
      Researching reasoning models, diffusion-based language models,
      and multi-modal understanding.
    </p>
    <ul class="r-social">
      <li><a href="/assets/cv_yoonjeon_kim.pdf"><i class="fas fa-file-alt"></i> CV</a></li>
      <li><a href="mailto:yoonkim313@kaist.ac.kr"><i class="fas fa-envelope"></i> Email</a></li>
      <li><a href="https://www.linkedin.com/in/yoonjeon-kim-9898061b0/"><i class="fab fa-linkedin"></i> LinkedIn</a></li>
      <li><a href="https://scholar.google.com/citations?user=E7CinH8AAAAJ&hl=en"><i class="fas fa-graduation-cap"></i> Scholar</a></li>
      <li><a href="https://github.com/akatigre"><i class="fab fa-github"></i> GitHub</a></li>
    </ul>
  </div>
</section>

<!-- ── SELECTED RESEARCH ──────────────────────────────────────── -->
<section class="r-section r-fade" id="research">
  <div class="r-section-head"><span class="r-label">Selected Research</span></div>
  <div class="r-cards">

    <article class="r-card">
      <div class="r-card-meta">
        <span class="r-badge r-badge-review">Under Review</span>
        <span class="r-card-year">2026</span>
      </div>
      <h2 class="r-card-title">Efficient Reinforcement for Visual-Textual Thinking with Discrete Diffusion Model</h2>
      <p class="r-card-summary">A diffusion-based RL framework for interleaved visual-textual reasoning. Localized visual editing reduces GRPO rollout computation by 26.9%; factorized reward assignment resolves cross-modal credit assignment, yielding 38% gains over SFT.</p>
      <p class="r-card-authors"><strong>Yoonjeon Kim</strong>, Yuhta Takida, Chieh-Hsin Lai, Eunho Yang, Yuki Mitsufuji</p>
      <div class="r-card-footer">
        <a class="r-link" href="https://drive.google.com/file/d/1h7yRqmKcIQcUClbH7h715Z77QWnCRB6n/view?usp=drive_link"><i class="fas fa-file-pdf"></i> paper</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
      </div>
      <div class="r-abs-body">Unified multimodal foundation models have enabled both visual understanding and generation within a single framework. Building on this foundation, supervised fine-tuning and reinforcement learning have been employed to facilitate interleaved visual and textual thinking, tightly coupling image generation with textual reasoning. Existing works predominantly rely on autoregressive unified models as the backbone, which incurs substantial computational overhead due to full regeneration of image token sequences at every rollout step. In this work, we instead leverage multimodal discrete diffusion models to develop a reinforcement learning framework for interleaved reasoning. By exploiting bidirectional context modeling, our approach enables <em>localized visual editing</em>, allowing targeted modifications and reducing rollout computation during GRPO by 26.9% compared to full-image editing baselines, with only a minimal performance drop. However, bidirectional multimodal decoding in discrete diffusion models introduces a non-trivial challenge: rewards become implicitly coupled across interleaved image and text tokens, leading to spurious cross-modal credit assignment. To address this, we propose <em>factorized reward assignment</em> across text and vision streams, assigning rewards to their corresponding token segments for stable credit propagation. This yields 11.2% gains over joint reward assignment baselines and 38.04% improvements over the supervised fine-tuned model.</div>
    </article>

    <article class="r-card">
      <div class="r-card-meta">
        <span class="r-badge r-badge-conf">ICML</span>
        <span class="r-card-year">2026</span>
      </div>
      <h2 class="r-card-title">Verifying Meta-Awareness via Predictive Rewards in Reasoning Models</h2>
      <p class="r-card-summary">Meta-awareness objectives let reasoning models self-predict rollout statistics — length, pass-rate, and concepts used — enabling 83% accuracy gains on AIME25 and a 1.28× GRPO training speedup.</p>
      <p class="r-card-authors"><strong>Yoonjeon Kim*</strong>, Doohyuk Jang*, Eunho Yang &nbsp;·&nbsp; *Equal Contribution</p>
      <div class="r-card-footer">
        <a class="r-link" href="https://drive.google.com/file/d/1n3cKn0jOWSnvmLhdUh2AxT3j3nbNnxVi/view?usp=drive_link"><i class="fas fa-file-pdf"></i> paper</a>
        <a class="r-link" href="https://github.com/akatigre/MASA-RL"><i class="fab fa-github"></i> code</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
        <button class="r-bib-btn" aria-expanded="false"><span class="r-bib-label">BibTeX</span></button>
      </div>
      <div class="r-abs-body">Recent research on reasoning models explores the meta-awareness of language models, including their ability to determine optimal thinking duration, recognize knowledge boundaries, and structure concept-level thinking. While current large reasoning models depend solely on answer-based verification, we show that adding meta-awareness objectives leads to significant performance gains over models without such meta-knowledge. MAPR utilizes a self-generated task of predicting rollout statistics — specifically length, pass-rate, and concepts used — allowing for verification against the actual statistics. Furthermore, by leveraging this self-predictive capability, the model can regulate its reasoning behavior by (i) filtering out trivial or unsolvable prompts, (ii) reducing lengthy generations that tend to be incorrect, and (iii) generating hints relevant to the problem. MAPR yields significant improvements in both accuracy and training efficiency on various reasoning benchmarks: a 1.28× GRPO training speedup, 83.18% gain in accuracy on AIME25, and 13.04% average gain over six mathematics benchmarks.</div>
      <div class="r-bib-body">
        <div class="r-bib-inner">
          <div class="r-bib-header">
            <span class="r-bib-label-sm">BibTeX</span>
            <button class="r-bib-copy" aria-label="Copy BibTeX to clipboard">Copy</button>
          </div>
          <code class="r-bib-code">@inproceedings{
anonymous2026verifying,
title={Verifying Meta-Awareness via Predictive Rewards in Reasoning Models},
author={Yoonjeon Kim, Doohyuk Jang, Eunho Yang},
booktitle={Forty-third International Conference on Machine Learning},
year={2026},
url={https://openreview.net/forum?id=Vl3tXPbjSH}
}</code>
        </div>
      </div>
    </article>

    <article class="r-card">
      <div class="r-card-meta">
        <span class="r-badge r-badge-conf">CVPR</span>
        <span class="r-card-year">2025</span>
      </div>
      <h2 class="r-card-title">Preserve or Modify? Context-Aware Evaluation for Balancing Preservation and Modification in Text-Guided Image Editing</h2>
      <p class="r-card-summary">AugCLIP derives an ideal-edit CLIP representation using an MLLM to adaptively coordinate preservation and modification — outperforming prior metrics across five benchmarks and aligning closely with human judgment.</p>
      <p class="r-card-authors"><strong>Yoonjeon Kim*</strong>, Soohyun Ryu*, Yeonsung Jung, Hyunkoo Lee, Joowon Kim, June Yong Yang, Jaeryong Hwang, Eunho Yang &nbsp;·&nbsp; *Equal Contribution</p>
      <div class="r-card-footer">
        <a class="r-link" href="https://arxiv.org/pdf/2410.11374"><i class="fas fa-file-pdf"></i> paper</a>
        <a class="r-link" href="https://github.com/augclip/augclip_eval"><i class="fab fa-github"></i> code</a>
        <a class="r-link" href="https://augclip.github.io/"><i class="fas fa-globe"></i> project</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
        <button class="r-bib-btn" aria-expanded="false"><span class="r-bib-label">BibTeX</span></button>
      </div>
      <div class="r-abs-body">The development of vision-language and generative models has significantly advanced text-guided image editing, which seeks the preservation of core elements in the source image while implementing modifications based on the target text. However, existing metrics have a context-blindness problem, indiscriminately applying the same evaluation criteria on completely different pairs of source image and target text, biasing towards either modification or preservation. Directional CLIP similarity, the only metric that considers both source image and target text, is also biased towards modification aspects. We propose AugCLIP, a context-aware metric that adaptively coordinates preservation and modification aspects depending on the specific context. This is done by deriving the CLIP representation of an ideally edited image using a multi-modal large language model to augment textual descriptions, then calculating a modification vector through a hyperplane that separates source and target attributes in CLIP space. Extensive experiments on five benchmark datasets show that AugCLIP aligns remarkably well with human evaluation standards, outperforming existing metrics.</div>
      <div class="r-bib-body">
        <div class="r-bib-inner">
          <div class="r-bib-header">
            <span class="r-bib-label-sm">BibTeX</span>
            <button class="r-bib-copy" aria-label="Copy BibTeX to clipboard">Copy</button>
          </div>
          <code class="r-bib-code">@InProceedings{Kim_2025_CVPR,
    author    = {Kim, Yoonjeon and Ryu, Soohyun and Jung, Yeonsung and Lee, Hyunkoo and Kim, Joowon and Yang, June Yong and Hwang, Jaeryong and Yang, Eunho},
    title     = {Preserve or Modify? Context-Aware Evaluation for Balancing Preservation and Modification in Text-Guided Image Editing},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2025},
    pages     = {23474-23483}
}</code>
        </div>
      </div>
    </article>

  </div>
</section>

<!-- ── NEWS ───────────────────────────────────────────────────── -->
<section class="r-section r-fade" id="news">
  <div class="r-section-head"><span class="r-label">News</span></div>
  <div class="r-news">
    <div class="r-news-item">
      <span class="r-news-date">May 2026</span>
      <span class="r-news-text">Paper accepted at <strong>ICML 2026</strong> — <em>Verifying Meta-Awareness via Predictive Rewards in Reasoning Models</em></span>
    </div>
    <div class="r-news-item">
      <span class="r-news-date">Jan 2026</span>
      <span class="r-news-text">Started Research Internship at <strong>SONY Research</strong>, Tokyo — mentored by <a href="https://scholar.google.com/citations?user=ahqdEYUAAAAJ&hl=ja">Yuhta Takida</a> and <a href="https://chiehhsinjesselai.github.io/">Chieh-Hsin (Jesse) Lai</a></span>
    </div>
    <div class="r-news-item">
      <span class="r-news-date">Feb 2025</span>
      <span class="r-news-text">Paper accepted at <strong>CVPR 2025</strong> — <em>Preserve or Modify?</em></span>
    </div>
    <div class="r-news-item">
      <span class="r-news-date">2024</span>
      <span class="r-news-text">Invited talk at <a href="https://www.kaist.ac.kr/news/html/news/?mode=V&mng_no=46270">AI Technology Seminar</a> hosted by KAIST AI Graduate School</span>
    </div>
  </div>
</section>

<!-- ── PUBLICATIONS ───────────────────────────────────────────── -->
<section class="r-section r-fade" id="publications">
  <div class="r-section-head"><span class="r-label">Publications</span></div>
  <div class="r-pub-list">

    <div class="r-pub">
      <h3 class="r-pub-title">Verifying Meta-Awareness via Predictive Rewards in Reasoning Models</h3>
      <p class="r-pub-authors"><strong>Yoonjeon Kim*</strong>, Doohyuk Jang*, Eunho Yang &nbsp;·&nbsp; *Equal Contribution</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-conf">ICML 2026</span>
        <a class="r-link" href="https://drive.google.com/file/d/1n3cKn0jOWSnvmLhdUh2AxT3j3nbNnxVi/view?usp=drive_link">paper</a>
        <a class="r-link" href="https://github.com/akatigre/MASA-RL">code</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
        <button class="r-bib-btn" aria-expanded="false"><span class="r-bib-label">BibTeX</span></button>
      </div>
      <div class="r-abs-body">Recent research on reasoning models explores the meta-awareness of language models, including their ability to determine optimal thinking duration, recognize knowledge boundaries, and structure concept-level thinking. While current large reasoning models depend solely on answer-based verification, we show that adding meta-awareness objectives leads to significant performance gains over models without such meta-knowledge. MAPR utilizes a self-generated task of predicting rollout statistics — specifically length, pass-rate, and concepts used — allowing for verification against the actual statistics. Furthermore, by leveraging this self-predictive capability, the model can regulate its reasoning behavior by (i) filtering out trivial or unsolvable prompts, (ii) reducing lengthy generations that tend to be incorrect, and (iii) generating hints relevant to the problem. MAPR yields significant improvements in both accuracy and training efficiency on various reasoning benchmarks: a 1.28× GRPO training speedup, 83.18% gain in accuracy on AIME25, and 13.04% average gain over six mathematics benchmarks.</div>
      <div class="r-bib-body">
        <div class="r-bib-inner">
          <div class="r-bib-header">
            <span class="r-bib-label-sm">BibTeX</span>
            <button class="r-bib-copy" aria-label="Copy BibTeX to clipboard">Copy</button>
          </div>
          <code class="r-bib-code">@inproceedings{
anonymous2026verifying,
title={Verifying Meta-Awareness via Predictive Rewards in Reasoning Models},
author={Yoonjeon Kim, Doohyuk Jang, Eunho Yang},
booktitle={Forty-third International Conference on Machine Learning},
year={2026},
url={https://openreview.net/forum?id=Vl3tXPbjSH}
}</code>
        </div>
      </div>
    </div>

    <div class="r-pub">
      <h3 class="r-pub-title">Efficient Reinforcement for Visual-Textual Thinking with Discrete Diffusion Model</h3>
      <p class="r-pub-authors"><strong>Yoonjeon Kim</strong>, Yuhta Takida, Chieh-Hsin Lai, Eunho Yang, Yuki Mitsufuji</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-review">Under Review</span>
        <a class="r-link" href="https://drive.google.com/file/d/1h7yRqmKcIQcUClbH7h715Z77QWnCRB6n/view?usp=drive_link">paper</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
      </div>
      <div class="r-abs-body">Unified multimodal foundation models have enabled both visual understanding and generation within a single framework. Building on this foundation, supervised fine-tuning and reinforcement learning have been employed to facilitate interleaved visual and textual thinking, tightly coupling image generation with textual reasoning. Existing works predominantly rely on autoregressive unified models as the backbone, which incurs substantial computational overhead due to full regeneration of image token sequences at every rollout step. In this work, we instead leverage multimodal discrete diffusion models to develop a reinforcement learning framework for interleaved reasoning. By exploiting bidirectional context modeling, our approach enables localized visual editing, allowing targeted modifications and reducing rollout computation during GRPO by 26.9% compared to full-image editing baselines. We propose factorized reward assignment across text and vision streams to address spurious cross-modal credit assignment, yielding 11.2% gains over joint reward baselines and 38.04% improvements over the supervised fine-tuned model.</div>
    </div>

    <div class="r-pub">
      <h3 class="r-pub-title">Reasoning Model is Stubborn: Diagnosing Instruction Overriding in Reasoning Models</h3>
      <p class="r-pub-authors">Doohyuk Jang*, <strong>Yoonjeon Kim*</strong>, Chanjae Park, Hyun Ryu, Eunho Yang &nbsp;·&nbsp; *Equal Contribution</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-review">Under Review</span>
        <a class="r-link" href="https://arxiv.org/abs/2505.17225">paper</a>
        <a class="r-link" href="https://github.com/ReasoningTrap/ReasoningTrap">code</a>
        <a class="r-link" href="https://reasoningtrap.github.io/">project</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
      </div>
      <div class="r-abs-body">Large reasoning models have demonstrated remarkable proficiency in various tasks. However, we observe that they frequently exhibit a problematic reliance on familiar reasoning patterns, a phenomenon we term reasoning rigidity. Despite explicit instructions from users, these models often override clearly stated conditions and default to habitual reasoning, leading to incorrect conclusions. This behavior presents significant challenges not only in reasoning-intensive domains but also in realistic settings. To systematically investigate reasoning rigidity, a behavior unexplored in prior work, we introduce a dataset, ReasoningTrap, including math problems, puzzles, and agentic tasks that diagnoses reasoning rigidity. Using this dataset, we identify patterns that occur when models default to ingrained reasoning, and suggest inference-level and GRPO-based post-training remedies. We will publicly release our diagnostic set to facilitate future research on mitigating reasoning rigidity in language models.</div>
    </div>

    <div class="r-pub">
      <h3 class="r-pub-title">Preserve or Modify? Context-Aware Evaluation for Balancing Preservation and Modification in Text-Guided Image Editing</h3>
      <p class="r-pub-authors"><strong>Yoonjeon Kim*</strong>, Soohyun Ryu*, Yeonsung Jung, Hyunkoo Lee, Joowon Kim, June Yong Yang, Jaeryong Hwang, Eunho Yang &nbsp;·&nbsp; *Equal Contribution</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-conf">CVPR 2025</span>
        <a class="r-link" href="https://arxiv.org/pdf/2410.11374">paper</a>
        <a class="r-link" href="https://github.com/augclip/augclip_eval">code</a>
        <a class="r-link" href="https://augclip.github.io/">project</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
        <button class="r-bib-btn" aria-expanded="false"><span class="r-bib-label">BibTeX</span></button>
      </div>
      <div class="r-abs-body">The development of vision-language and generative models has significantly advanced text-guided image editing, which seeks the preservation of core elements in the source image while implementing modifications based on the target text. However, existing metrics have a context-blindness problem, indiscriminately applying the same evaluation criteria on completely different pairs of source image and target text, biasing towards either modification or preservation. We propose AugCLIP, a context-aware metric that adaptively coordinates preservation and modification aspects depending on the specific context of a given source image and target text. This is done by deriving the CLIP representation of an ideally edited image using a multi-modal large language model to augment textual descriptions, then calculating a modification vector through a hyperplane that separates source and target attributes in CLIP space. Extensive experiments on five benchmark datasets show that AugCLIP aligns remarkably well with human evaluation standards, outperforming existing metrics.</div>
      <div class="r-bib-body">
        <div class="r-bib-inner">
          <div class="r-bib-header">
            <span class="r-bib-label-sm">BibTeX</span>
            <button class="r-bib-copy" aria-label="Copy BibTeX to clipboard">Copy</button>
          </div>
          <code class="r-bib-code">@InProceedings{Kim_2025_CVPR,
    author    = {Kim, Yoonjeon and Ryu, Soohyun and Jung, Yeonsung and Lee, Hyunkoo and Kim, Joowon and Yang, June Yong and Hwang, Jaeryong and Yang, Eunho},
    title     = {Preserve or Modify? Context-Aware Evaluation for Balancing Preservation and Modification in Text-Guided Image Editing},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2025},
    pages     = {23474-23483}
}</code>
        </div>
      </div>
    </div>

    <div class="r-pub">
      <h3 class="r-pub-title">Learning Input-agnostic Manipulation Directions in StyleGAN with Text Guidance</h3>
      <p class="r-pub-authors"><strong>Yoonjeon Kim</strong>, Hyunsu Kim, Junho Kim, Yunjey Choi, Eunho Yang</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-conf">ICLR 2023</span>
        <a class="r-link" href="https://openreview.net/forum?id=47B_ctC4pJ">paper</a>
        <button class="r-abs-btn" aria-expanded="false"><span class="r-toggle-label">Abstract +</span></button>
        <button class="r-bib-btn" aria-expanded="false"><span class="r-bib-label">BibTeX</span></button>
      </div>
      <div class="r-abs-body">With the advantages of fast inference and human-friendly flexible manipulation, image-agnostic style manipulation via text guidance enables new applications that were not previously available. The state-of-the-art text-guided image-agnostic manipulation method embeds the representation of each channel of StyleGAN independently in the CLIP space, and provides it in the form of a Dictionary to quickly find the channel-wise manipulation direction during inference. However, this dictionary — constructed by controlling single channels individually — is limited in accommodating the versatility of text guidance since the collective and interactive relation among multiple channels is not considered. Indeed, it fails to discover a large portion of manipulation directions that can be found by existing methods which manually manipulate the latent space without texts. To alleviate this, we propose a novel method that learns a Dictionary whose entry corresponds to the representation of a single channel by taking into account the manipulation effect coming from the interaction with multiple other channels. We demonstrate that our strategy resolves the inability of previous methods in finding diverse known directions from unsupervised methods and unknown directions from random text, while maintaining real-time inference speed and disentanglement ability.</div>
      <div class="r-bib-body">
        <div class="r-bib-inner">
          <div class="r-bib-header">
            <span class="r-bib-label-sm">BibTeX</span>
            <button class="r-bib-copy" aria-label="Copy BibTeX to clipboard">Copy</button>
          </div>
          <code class="r-bib-code">@inproceedings{
kim2023learning,
title={Learning Input-agnostic Manipulation Directions in Style{GAN} with Text Guidance},
author={Yoonjeon Kim and Hyunsu Kim and Junho Kim and Yunjey Choi and Eunho Yang},
booktitle={The Eleventh International Conference on Learning Representations},
year={2023},
url={https://openreview.net/forum?id=47B_ctC4pJ}
}</code>
        </div>
      </div>
    </div>

    <div class="r-pub">
      <h3 class="r-pub-title">Sequential Targeting: A Continual Learning Approach for Data Imbalance in Text Classification</h3>
      <p class="r-pub-authors">Joel Jang, <strong>Yoonjeon Kim</strong>, Kyoungho Choi, Sungho Suh</p>
      <div class="r-pub-row">
        <span class="r-badge r-badge-journal">Expert Systems with Applications 2021</span>
        <a class="r-link" href="https://www.sciencedirect.com/science/article/abs/pii/S095741742100508X">paper</a>
      </div>
    </div>

  </div>
</section>

<!-- ── TALKS ──────────────────────────────────────────────────── -->
<section class="r-section r-fade" id="talks">
  <div class="r-section-head"><span class="r-label">Talks</span></div>
  <div class="r-talks">
    <div class="r-talk">
      <div class="r-talk-icon"><i class="fas fa-microphone-alt"></i></div>
      <div class="r-talk-body">
        <p class="r-talk-title">AI Technology Seminar — KAIST AI Graduate School</p>
        <a class="r-talk-link" href="https://www.kaist.ac.kr/news/html/news/?mode=V&mng_no=46270">↗ view announcement</a>
      </div>
    </div>
  </div>
</section>

<!-- ── PROJECTS ───────────────────────────────────────────────── -->
<section class="r-section r-fade" id="projects">
  <div class="r-section-head"><span class="r-label">Projects</span></div>
  <div class="r-proj-list">
    <div class="r-proj">
      <div class="r-proj-funder">National Research Foundation of Korea</div>
      <div class="r-proj-name">A Study on Optimization and Network Interpretation Method for Large-Scale Machine Learning</div>
      <div class="r-proj-period">Mar 2024 – Feb 2027</div>
    </div>
    <div class="r-proj">
      <div class="r-proj-funder">Intel Corporation &amp; NAVER</div>
      <div class="r-proj-name">Efficient Foundation Models on Intel Systems</div>
      <div class="r-proj-period">Sep 2024 – Aug 2027</div>
    </div>
    <div class="r-proj">
      <div class="r-proj-funder">NAVER Cloud</div>
      <div class="r-proj-name">Naver-KAIST Hyper-Creative Center</div>
      <div class="r-proj-period">Sep 2021 – Aug 2023</div>
    </div>
  </div>
</section>

<!-- ── EXPERIENCE ─────────────────────────────────────────────── -->
<section class="r-section r-fade" id="experience">
  <div class="r-section-head"><span class="r-label">Experience</span></div>

  <div class="r-timeline">
    <div class="r-tl-item">
      <div class="r-tl-date">Jan 2026 – Jun 2026 &nbsp;·&nbsp; Ongoing</div>
      <div class="r-tl-org">SONY Research</div>
      <div class="r-tl-role">Research Intern &nbsp;·&nbsp; Tokyo, Japan</div>
      <div class="r-tl-detail">
        Mentored by <a href="https://scholar.google.com/citations?user=ahqdEYUAAAAJ&hl=ja">Yuhta Takida</a> and <a href="https://chiehhsinjesselai.github.io/">Chieh-Hsin (Jesse) Lai</a>.
        <ul class="r-tl-sub">
          <li>Multi-modal Discrete Diffusion Model</li>
          <li>Reinforcement Learning on Multi-modal Reasoning</li>
        </ul>
      </div>
    </div>
    <div class="r-tl-item">
      <div class="r-tl-date">Jul 2023 – Oct 2023</div>
      <div class="r-tl-org">NAVER Cloud</div>
      <div class="r-tl-role">Research Intern</div>
    </div>
  </div>

  <div class="r-sub-head"><span class="r-label">Education</span></div>
  <div class="r-edu-list">
    <div class="r-edu-item">
      <span class="r-edu-deg">Ph.D.</span>
      <div>
        <div class="r-edu-inst">Korea Advanced Institute of Science and Technology (KAIST)</div>
        <div class="r-edu-dept">Graduate School of AI</div>
        <div class="r-edu-period">Mar 2023 – Present</div>
      </div>
    </div>
    <div class="r-edu-item">
      <span class="r-edu-deg">M.S.</span>
      <div>
        <div class="r-edu-inst">Korea Advanced Institute of Science and Technology (KAIST)</div>
        <div class="r-edu-dept">Graduate School of AI</div>
        <div class="r-edu-period">Mar 2021 – Feb 2023</div>
      </div>
    </div>
    <div class="r-edu-item">
      <span class="r-edu-deg">B.S.</span>
      <div>
        <div class="r-edu-inst">Yonsei University</div>
        <div class="r-edu-dept">Applied Statistics</div>
        <div class="r-edu-period">Mar 2017 – Feb 2021</div>
      </div>
    </div>
  </div>

  <div class="r-service">
    <div class="r-service-label">Academic Service &nbsp;·&nbsp; Conference Reviewer</div>
    <div class="r-chips">
      <span class="r-chip">ICLR</span>
      <span class="r-chip">CVPR</span>
      <span class="r-chip">NeurIPS</span>
    </div>
  </div>

</section>
