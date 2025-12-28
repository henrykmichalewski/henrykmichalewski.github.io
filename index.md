---
layout: homepage
---

<style>
/* Minimal Tab Style */
.tab {
  overflow: hidden;
  margin-top: 20px;
  margin-bottom: 20px;
  border-bottom: 1px solid #e5e5e5; /* Light mode border */
}

.tab button {
  background-color: transparent;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 10px 10px;
  transition: 0.3s;
  font-size: 13px;
  font-family: inherit; /* Use theme font */
  color: #595959; /* Default text color */
  font-weight: 500;
  border-bottom: 2px solid transparent;
}

.tab button:hover {
  color: #043361;
}

.tab button.active {
  color: #043361;
  border-bottom: 2px solid #043361;
}

.tabcontent {
  display: none;
  padding: 20px 0; /* Remove side padding, add top/bottom */
  border: none;
  animation: fadeEffect 0.5s; /* Add fade effect */
}

@keyframes fadeEffect {
  from {opacity: 0;}
  to {opacity: 1;}
}

/* Dark Mode */
@media (prefers-color-scheme: dark) {
  .tab {
    border-bottom: 1px solid #444;
  }
  .tab button {
    color: #dadbdf;
  }
  .tab button:hover {
    color: rgb(62, 183, 240);
  }
  .tab button.active {
    color: rgb(62, 183, 240);
    border-bottom: 2px solid rgb(62, 183, 240);
  }
}
</style>

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'WorkEngagements')" id="defaultOpen">Bio and Work Engagements</button>
  <button class="tablinks" onclick="openTab(event, 'OpenSource')">Open Source</button>
  <button class="tablinks" onclick="openTab(event, 'SelectedPapers')">Selected Papers</button>
  <button class="tablinks" onclick="openTab(event, 'Patents')">Selected Patents</button>
  <button class="tablinks" onclick="openTab(event, 'Education')">Education</button>
  <button class="tablinks" onclick="openTab(event, 'Mentoring')">Mentoring</button>
</div>


<div id="WorkEngagements" class="tabcontent" markdown="1">

## Bio

Prior to 2015, my research focused on pure mathematics and theoretical computer science, covering logic, foundations, game theory, and optimization. I subsequently pivoted to work exclusively on machine learning. Throughout my career, I have been fortunate to interact with leadership that supported new research directions and collaborate with exceptional researchers who made it possible to pursue these directions.

Before joining Google in 2019, I worked on [reinforcement learning for theorem proving](https://proceedings.neurips.cc/paper/8098-reinforcement-learning-of-theorem-proving.pdf), a [sim2real project with Volkswagen](https://www.mimuw.edu.pl/~henrykm/pubs_2019/sim2real_outdoor.pdf), and [model-based RL](https://arxiv.org/abs/1903.00374). At Google, I have contributed to [PaLM](https://arxiv.org/abs/2204.02311), [early program synthesis work with LLMs](https://arxiv.org/abs/2108.07732), [Scratchpad](https://arxiv.org/abs/2112.00114), and [Minerva](https://arxiv.org/abs/2206.14858). More recently, I worked on the [math-specialized model presented in the Gemini 1.5 report](https://storage.googleapis.com/deepmind-media/gemini/gemini_v1_5_report.pdf), [Big Sleep](https://googleprojectzero.blogspot.com/2024/10/from-naptime-to-big-sleep.html), [AlphaProof](https://www.nature.com/articles/s41586-025-09833-y), and all iterations of the main Gemini models. Leveraging Google’s infrastructure, I have conducted thousands of experiments and submitted over 1,000 pull requests—roughly half of which were to the Gemini codebase.

## Work Engagements

<style>
.work-img {
  width: 140px;
  height: 60px;
  object-fit: contain;
  margin-right: 15px;
  vertical-align: middle;
  background-color: transparent;
  padding: 0;
  box-shadow: none;
}
@media (prefers-color-scheme: dark) {
  .work-img {
    background-color: transparent;
    opacity: 1.0;
  }
}
</style>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/google_deepmind.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Senior Staff Research Scientist</div>
    <div class="periodical"><em>Google DeepMind, 2025–present</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/google_deepmind.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Staff Research Scientist</div>
    <div class="periodical"><em>Google DeepMind, 2023–2025</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/google.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Staff Research Scientist</div>
    <div class="periodical"><em>Google Brain, 2021–2023</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/oxford.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Leverhulme Fellow</div>
    <div class="periodical"><em>Department of Computer Science, University of Oxford, 2021–2022</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/google.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Visiting Researcher (Staff Faculty Visiting Researcher)</div>
    <div class="periodical"><em>Google, 2019–2021</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/oxford.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Visiting Researcher</div>
    <div class="periodical"><em>Department of Computer Science, University of Oxford, 2018–2019</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/ens.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Invited Professor</div>
    <div class="periodical"><em>École normale supérieure de Lyon, 2017</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/deepsense_new_inverted.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Data Scientist</div>
    <div class="periodical"><em>deepsense.ai, 2016–2019</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/uw_custom.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Associate Professor (last held position)</div>
    <div class="periodical"><em>University of Warsaw, 2007–present, on a long term leave since 2016</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/bgu.svg" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Postdoctoral Researcher</div>
    <div class="periodical"><em>Ben-Gurion University, Israel, 2004–2007</em></div>
  </div>
</div>

</div>

<div id="OpenSource" class="tabcontent" markdown="1">

## Open Source Contributions

- **[Trax](https://github.com/google/trax)** — contributions to sequence modeling, training pipelines, and reasoning-focused components.  
- **[Formal Putnam-like Benchmark](https://github.com/google-deepmind/formal-putnam-like)** — co-developer of an olympiad-level mathematical reasoning evaluation suite.  
- **[Eval-Hub](https://github.com/google-deepmind/eval_hub)** — contributor to a unified evaluation framework for LLM reasoning, code generation, and multimodal tasks.  

</div>

<div id="SelectedPapers" class="tabcontent" markdown="1">


<style>
.teaser-img {
  width: 160px;
  height: 80px;
  object-fit: cover;
  border-radius: 8px;
  box-shadow: 3px 3px 6px #888;
  margin-right: 10px;
  vertical-align: middle;
  background-color: transparent;
}
@media (prefers-color-scheme: dark) {
  .teaser-img {
    box-shadow: 3px 3px 6px #000;
  }
}
</style>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/alphaproof_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://www.nature.com/articles/s41586-025-09833-y">Olympiad-level formal mathematical reasoning with reinforcement learning</a></div>
    <div class="periodical"><em>Nature 2025</em></div>
    <div class="links">
      <a href="https://www.nature.com/articles/s41586-025-09833-y_reference.pdf" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/beyond_lines_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://aclanthology.org/2024.findings-emnlp.360/">Beyond Lines and Circles: Unveiling the Geometric Reasoning Gap in Large Language Models</a></div>
    <div class="periodical"><em>EMNLP 2024</em></div>
    <div class="links">
      <a href="https://aclanthology.org/2024.findings-emnlp.360/" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/promptbreeder_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://icml.cc/virtual/2024/poster/34801">Promptbreeder: Self-Referential Self-Improvement via Prompt Evolution</a></div>
    <div class="periodical"><em>ICML 2024</em></div>
    <div class="links">
      <a href="https://icml.cc/virtual/2024/poster/34801" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/focused_transformer_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://openreview.net/forum?id=s1FjXzJ0jy&noteId=PjanKdC3Ka">Focused Transformer: Contrastive Training for Context Scaling</a></div>
    <div class="periodical"><em>NeurIPS 2023</em></div>
    <div class="links">
      <a href="https://openreview.net/forum?id=s1FjXzJ0jy&noteId=PjanKdC3Ka" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/rt2_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/2307.15818">RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control</a></div>
    <div class="periodical"><em>ArXiv 2023</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/2307.15818" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/minerva_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://papers.nips.cc/paper_files/paper/2022/hash/18abbeef8cfe9203fdf9053c9c4fe191-Abstract-Conference.html">Solving Quantitative Reasoning Problems with Language Models</a></div>
    <div class="periodical"><em>NeurIPS 2022</em></div>
    <div class="links">
      <a href="https://papers.nips.cc/paper_files/paper/2022/hash/18abbeef8cfe9203fdf9053c9c4fe191-Abstract-Conference.html" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/multi_game_dt_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/2205.15241">Multi-Game Decision Transformers</a></div>
    <div class="periodical"><em>ArXiv 2022</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/2205.15241" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/hierarchical_transformer_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://aclanthology.org/2022.findings-naacl.117/">Hierarchical Transformers Are More Efficient Language Models</a></div>
    <div class="periodical"><em>NAACL 2022 (Findings)</em></div>
    <div class="links">
      <a href="https://aclanthology.org/2022.findings-naacl.117/" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/program_synthesis_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/2108.07732">Program Synthesis with Large Language Models</a></div>
    <div class="periodical"><em>ArXiv 2021</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/2108.07732" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/scratchpad_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/2112.00114">Show Your Work: Scratchpads for Intermediate Computation with Language Models</a></div>
    <div class="periodical"><em>ArXiv 2021</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/2112.00114" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/rl_theorem_proving_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://papers.nips.cc/paper/8098-reinforcement-learning-of-theorem-proving">Reinforcement Learning of Theorem Proving</a></div>
    <div class="periodical"><em>NeurIPS 2018</em></div>
    <div class="links">
      <a href="https://papers.nips.cc/paper/8098-reinforcement-learning-of-theorem-proving" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/sim2real_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://www.mimuw.edu.pl/~henrykm/pubs_2019/sim2real_outdoor.pdf">Sim2Real Autonomous Driving</a></div>
    <div class="periodical"><em>ICRA 2020</em></div>
    <div class="links">
      <a href="https://www.mimuw.edu.pl/~henrykm/pubs_2019/sim2real_outdoor.pdf" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/model_based_rl_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/1903.00374">Model-Based RL for Atari</a></div>
    <div class="periodical"><em>ICLR 2020</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/1903.00374" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>


<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/bert_math_reasoning_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/2106.03921">Measuring and Improving BERT’s Mathematical Abilities by Predicting the Order of Reasoning</a></div>
    <div class="periodical"><em>ACL 2021</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/2106.03921" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/mso_u_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://link.springer.com/chapter/10.1007/978-3-662-43951-7_5">MSO+U on Infinite Trees</a></div>
    <div class="periodical"><em>ICALP 2014</em></div>
    <div class="links">
      <a href="https://link.springer.com/chapter/10.1007/978-3-662-43951-7_5" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/rabin_theorem_teaser.png" class="teaser-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="https://arxiv.org/abs/1508.06780">Logical Strength of Rabin’s Theorem</a></div>
    <div class="periodical"><em>LICS 2015</em></div>
    <div class="links">
      <a href="https://arxiv.org/abs/1508.06780" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    </div>
  </div>
</div>
<br>

</div>

<div id="Patents" class="tabcontent" markdown="1">

## Patents based on the [Scratchpad paper](https://arxiv.org/abs/2112.00114) contributions

- [Prompting Machine-Learned Models Using Chains of Thought](https://patents.google.com/patent/US20230394328A1/en) — chain-of-thought prompting and consistency-based selection of model outputs for improved reasoning robustness.  

- [Using Chains of Thought to Prompt Machine-Learned Models Pre-Trained on Diversified Objectives](https://patents.google.com/patent/US20230244938A1/en) — construction of instructive query–answer–reasoning triples for steering large pre-trained models via chain-of-thought prompts.
  

</div>

<div id="Education" class="tabcontent" markdown="1">

## Education

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/uw_custom.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Habilitation in Computer Science</div>
    <div class="periodical"><em>University of Warsaw, 2015</em></div>
    <div class="links">
      <a href="http://duch.mimuw.edu.pl/~henrykm/pubs_other/autoreferat_en.pdf" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Thesis</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/fields.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Internship</div>
    <div class="periodical"><em>Fields Institute, Toronto, Winter 2002</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/uw_custom.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">PhD in Mathematics</div>
    <div class="periodical"><em>University of Warsaw, 1998–2002</em></div>
    <div class="links">
      <a href="http://duch.mimuw.edu.pl/~henrykm/pubs_other/phd_thesis.ps" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Thesis</a>
    </div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/vu_processed.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">Internship</div>
    <div class="periodical"><em>Vrije University, Amsterdam, 1998</em></div>
  </div>
</div>
<br>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/logos/uw_custom.png" class="work-img">
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">MA in Mathematics</div>
    <div class="periodical"><em>University of Warsaw, 1993–1998</em></div>
    <div class="links">
      <a href="https://www.mimuw.edu.pl/~henrykm/pubs_other/ma_thesis.pdf" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Thesis</a>
    </div>
  </div>
</div>

</div>

<div id="Mentoring" class="tabcontent" markdown="1">

## Mentoring of Students

[Spyridon Mouselinos](https://spyrosmouselinos.github.io/), 2021–2025, Ph.D. project  
*[Towards Visual Reasoning](https://sites.google.com/view/visualreasoning/home)*,  
co-supervised with Mateusz Malinowski (Google DeepMind).

[Cécilia Pradic](https://www.swansea.ac.uk/staff/c.pradic/#publications=is-expanded), 2014–2019, PhD thesis  
*[Some proof-theoretical approaches to Monadic Second-Order logic](https://theses.hal.science/tel-02954006v1)*,  
co-supervised with [Colin Riba](https://perso.ens-lyon.fr/colin.riba/) (ENS Lyon).

</div>

<script>
function openTab(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
