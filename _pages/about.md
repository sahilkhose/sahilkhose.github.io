---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I am a Ph.D. student in Computer Science at <b>Georgia Tech</b>, where I have the privilege of being advised by <a href="https://faculty.cc.gatech.edu/~judy/" target="_blank"><b>Prof. Judy Hoffman</b></a>. Before this, I completed my M.S. at <b>Georgia Tech</b> and earned my B.Tech. from <b>Manipal Institute of Technology</b>, where I was mentored by Prof. Harish Kumar JR. I have also interned at IISc Bangalore, collaborating with Dr. Chandan Gautam and Prof. Suresh Sundaram. During my undergraduate years, I was actively involved in Project MANAS and the Research Society Manipal.

<div style="margin:1.5em 0 1em 0;">
  <span style="font-size:1.2em; font-weight:bold; color:#228be6;">Recent Projects</span>
  <ul style="margin-top:0.5em;">
    <li><b>World Models (WFM):</b> Developing VLM-based benchmarks for automatic evaluation of world models.</li>
    <li><b>7B Open-Source VLM:</b> Open-vocabulary 3D scene graph generation <span style="color:#868e96;">(under review)</span>.</li>
    <li><b>SkyScenes:</b> Synthetic aerial dataset for real-world segmentation <span style="color:#228be6;">(ECCV 2024)</span>.</li>
    <li><b>Generalist Multimodal LLM:</b> Jointly-trained vision-audio model that reduces cross-modal interference and outperforms larger models.</li>
  </ul>
</div>

My research advances <b>vision-language models (VLMs)</b> by extending their capabilities across modalities, spatial reasoning, and evaluation—integrating <b>audio</b>, enhancing <b>spatial understanding</b>, and enabling automatic evaluation of <b>world models</b> for robotic manipulation. I have also worked on <b>syn-to-real transfer</b> and <b>domain generalization</b>.

<!-- I regularly review for top conferences (NeurIPS, CVPR, ECCV) and have published in both vision and language communities. -->

<div style="margin:1.5em 0;">
  <blockquote style="background:#fff0f6; border-left:4px solid #d6336c; padding:0.8em 1em; font-size:1.08em;">
    💼 <span style="color:#d6336c; font-weight:bold;">I'm currently seeking research internships for 2026 — feel free to reach out if you're hiring!</span>
  </blockquote>
</div>

---

## 📝 Recent Updates <span style="font-size:small;">[ <b>🌟</b>: Highlight &nbsp;|&nbsp; <b>💡</b>: Research &nbsp;|&nbsp; <b>📆</b>: Misc ]</span>

<ul style="list-style-type:none; padding-left:0; margin-bottom:0.5em;">
  <li>
    <span style="font-size:1.1em;">🌟</span> <b>Attending CVPR 2025</b> in Nashville!
  </li>
  <li>
    <span style="font-size:1.1em;">🌟</span> <b>Attending ECCV 2024</b> in Milan, Italy!<br>
    <span style="font-size:0.97em;">Georgia Tech published an <a href="https://www.cc.gatech.edu/news/skyscenes-dataset-could-lead-safe-reliable-autonomous-flying-vehicles">article</a> about our work.</span>
  </li>
  <li>
    <span style="font-size:1.1em;">💡</span> <b>Jul 1, 2024:</b> My first first-author paper — <a href="https://arxiv.org/abs/2312.06719">SkyScenes: A Synthetic Dataset for Aerial Scene Understanding</a> — accepted at ECCV 2024!
  </li>
</ul>

<details>
  <summary style="cursor:pointer; font-weight:bold;">View more</summary>
  <ul style="list-style-type:none; padding-left:0; margin-top:0.5em;">
    <li>
      <span style="font-size:1.1em;">🌟</span> <b>Apr 1, 2024:</b> Joining Georgia Tech for Ph.D. CS under <b>Prof. Judy Hoffman</b> (Fall 2024).
    </li>
    <li>
      <span style="font-size:1.1em;">📆</span> <b>Mar 12, 2024:</b> Serving as a reviewer for ECCV 2024.
    </li>
    <li>
      <span style="font-size:1.1em;">💡</span> <b>Oct 24, 2023:</b> My first main-conference paper — <a href="https://arxiv.org/abs/2308.14596">LatentDR: Improving Model Generalization Through Sample-Aware Latent Degradation and Restoration</a> — accepted at WACV 2024!
    </li>
    <li>
      <span style="font-size:1.1em;">🌟</span> Attended NeurIPS 2022 in New Orleans, LA, USA (my first in-person conference!).
    </li>
    <li>
      <span style="font-size:1.1em;">🌟</span> <b>Apr 4, 2022:</b> Admitted to the <a href="https://www.cc.gatech.edu/degree-programs/master-science-computer-science">MS CS</a> program at <a href="https://www.gatech.edu/">Georgia Tech</a> for Fall 2022!
    </li>
  </ul>
</details>

---

## 📚 Publications

### <span style="color:#228be6;">2024</span>

#### <span style="color:#d6336c;">ECCV 2024</span> <span style="font-size:0.95em;">(First first-author paper!)</span>
<div style="background:#f8f9fa; border-radius:8px; padding:1em; margin-bottom:1em;">
  <b>SkyScenes: A Synthetic Dataset for Aerial Scene Understanding</b><br>
  <sub>Sahil Khose<sup>*</sup>, Anisha Pal<sup>*</sup>, Aayushi Agarwal<sup>*</sup>, Deepanshi<sup>*</sup>, Judy Hoffman, Prithvijit Chattopadhyay</sub>
  <div style="margin:0.5em 0;">
    <a href="https://arxiv.org/abs/2312.06719">[Paper]</a>
    <a href="https://hoffman-group.github.io/SkyScenes/">[Website]</a>
    <a href="https://huggingface.co/datasets/hoffman-lab/SkyScenes">[HF🤗]</a>
    <a href="https://www.cc.gatech.edu/news/skyscenes-dataset-could-lead-safe-reliable-autonomous-flying-vehicles">[CoC Article]</a>
    <a href="https://github.com/hoffman-group/SkyScenes">[GitHub]</a>
  </div>
  <img src="/images/skyscenes.png" alt="SkyScenes Sample" style="max-width:400px; border-radius:8px; margin-bottom:0.5em; box-shadow:0 2px 8px rgba(0,0,0,0.08);"/>
</div>

#### <span style="color:#228be6;">WACV 2024</span> <span style="font-size:0.95em;">(First main-conference paper!)</span>
<div style="background:#f8f9fa; border-radius:8px; padding:1em; margin-bottom:1em;">
  <b>LatentDR: Improving Model Generalization Through Sample-Aware Latent Degradation and Restoration</b><br>
  <sub>Ran Liu, Sahil Khose, Jingyun Xiao, Lakshmi Sathidevi, Keerthan Ramnath, Zsolt Kira, Eva L. Dyer</sub>
  <div style="margin:0.5em 0;">
    <a href="https://arxiv.org/abs/2308.14596">[Paper]</a>
  </div>
  <img src="./images/latentdr.png" alt="LatentDR Sample" style="max-width:400px; border-radius:8px; margin-bottom:0.5em; box-shadow:0 2px 8px rgba(0,0,0,0.08);"/>
</div>

---

### <span style="color:#fab005;">2022</span>

#### NeurIPS 2022 <span style="color:#fab005;">(First in-person conference!)</span>
- <strong>Poster:</strong> <a href="https://arxiv.org/abs/2209.10320">Continual VQA for Disaster Response Systems</a> at <a href="https://www.climatechange.ai/events/neurips2022">CCAI</a>

#### ICML 2022 <span style="color:#40c057;">(Best Paper Award 🌟)</span>
- <a href="https://arxiv.org/abs/2205.15025">An Efficient Modern Baseline for FloodNet VQA</a> at <a href="https://ablacan.github.io/NewInML2022_ICML/">New In ML</a>

#### ACL 2022
- <strong>Oral:</strong> <a href="https://arxiv.org/abs/2203.11899">Transformer based ensemble for emotion detection</a> at <a href="https://wassa-workshop.github.io/">WASSA</a>

---

### <span style="color:#fab005;">2021</span>

#### NeurIPS 2021
- <strong>Spotlight Paper 🌟:</strong> <a href="https://arxiv.org/abs/2105.08655">Semi-Supervised Classification and Segmentation on High Resolution Aerial Images</a> at <a href="https://www.climatechange.ai/events/neurips2021.html">CCAI</a>
- <a href="https://arxiv.org/abs/2108.11554">XCI-Sketch: Extraction of Color Information from Images for Generation of Colored Outlines and Sketches</a>  
  <sub>Presented at: New in ML (Oral), CtrlGen, ML4CD, and DGM</sub>
- <strong>Poster:</strong> <a href="https://arxiv.org/abs/2109.08924">A Studious Approach to Semi-Supervised Learning</a> at <a href="https://i-cant-believe-its-not-better.github.io/neurips2021/">ICBINB</a>

#### NAACL 2021 <span style="color:#fab005;">(Top Performer Award 🌟)</span>
- <a href="https://aclanthology.org/2021.smm4h-1.5/">BERT based Transformers lead the way in Extraction of Health Information from Social Media</a> at <a href="https://healthlanguageprocessing.org/smm4h-2021/">SMM4H</a>