---
layout: default
---

## Projects

### Recurrent LidarNet
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/re1null0)
*Python, PyTorch, CUDA, ROS2*

Extended 1D-CNN TinyLidarNet with a bidirectional LSTM + self-attention module, lifting lap-completion reliability from 30–78% to 90% on F1TENTH tracks and cutting average lap times by 11%. Quantized to TFLite INT8 (XNNPACK) and TensorRT FP16, achieving < 3 ms CPU and < 0.6 ms GPU inference while maintaining full generalization across novel tracks.

<div class="video-container">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/faTilMYMT5o" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<style>
.video-container {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
  max-width: 100%;
  margin-bottom: 20px;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>

### AirTwin
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/re1null0)
*Python, YOLO5, Point Cloud Processing, OpenCV, PyTorch, dust3r*

Engineered GPU-accelerated camera-based 3D reconstruction to deliver on-site digital twins in <1 s (20× faster vs. dust3r); fused LiDAR + camera for SLAM mapping; utilized RL wildfire-spread model to generate real-time threat maps, boosting unburned-area preservation to 70.15% from 11.76%.
<div class="video-container">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/98ngpQQqQg4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<style>
.video-container {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
  max-width: 100%;
  margin-bottom: 20px;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>

### Beyond School
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/re1null0)
*Python, OpenCV, YOLO*

Produced the first public curriculum on Neural Networks and Computer Vision (OpenCV) for 500+ learners. Designed presentations and devised scripts for over 15 YouTube video-lessons with 7500+ views.
<style>
.playlist-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-bottom: 30px;
}

.playlist-item {
  flex: 1;
  min-width: 300px;
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
}

.playlist-item iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

@media (max-width: 768px) {
  .playlist-item {
    flex: 100%;
  }
}
</style>

<div class="playlist-container">
  <div class="playlist-item">
    <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/videoseries?list=PLVFGVo0DNh5cAH3Cb0cl9ruli4RNNtaSF" title="YouTube playlist" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  
  <div class="playlist-item">
    <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/videoseries?list=PLVFGVo0DNh5duhps6KsiCQIoObyzcM2Cs" title="YouTube playlist" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>
---

## Research Experience

### Institute of Smart Systems and Artificial Intelligence | Research Intern
*Jun 2021 – Aug 2021*

- Simulated vaccination policies using agent-based modeling to identify the most effective strategies for reducing disease transmission; modeled sterilizing and effective immunization outcomes by adding 4 new SEIR states


### Yale School of Medicine | Research Assistant
*Jul 2020 – Jun 2021*

- Developed analysis on lung cancer survivability with 94% accuracy; implemented a novel approach to incorporate quantitative and qualitative multivariate analysis using Python and TCGA on 20 Gigabytes PET/CT scans, leading to significant differentiation between lung squamous cell carcinoma and adenocarcinoma

---
## Publications

<div class="publications">

  <div class="pub-entry">
    <span class="badge">npj Precision Oncology</span>
    <h3>Multimodal analysis suggests differential immuno-metabolic crosstalk in lung squamous cell carcinoma and adenocarcinoma</h3>
    <p>Brooks P. Leitner, Kevin B. Givechian, Shyryn Ospanova, Aray Beisenbayeva, Katerina Politi, Rachel J. Perry, et al.</p>
    <p><em>npj Precision Oncology, published 27 January 2022</em></p>
    <p><a class="btn" href="https://www.nature.com/articles/s41698-021-00248-2" target="_blank">View article</a></p>
  </div>

  <div class="pub-entry">
    <span class="badge">IEEE J Biomed Health Inform</span>
    <h3>A Vaccination Simulator for COVID-19: Effective and Sterilizing Immunization Cases</h3>
    <p>Aknur Karabay, Askat Kuzdeuov, Shyryn Ospanova, Michael Lewis, Huseyin Atakan Varol</p>
    <p><em>IEEE Journal of Biomedical and Health Informatics, December 2021</em></p>
    <p><a class="btn" href="https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9542855" target="_blank">View article</a></p>
  </div>

  <div class="pub-entry">
    <span class="badge">PLOS ONE</span>
    <h3>The impact of variance in carnitine palmitoyltransferase-1 expression on breast cancer prognosis is stratified by clinical and anthropometric factors</h3>
    <p>Ryan Liu, Shyryn Ospanova, Rachel J. Perry</p>
    <p><em>PLoS ONE 18(2): e0281252, published 3 February 2023</em></p>
    <p><a class="btn" href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0281252" target="_blank">View article</a></p>
  </div>

</div>

<style>/* Add to your main stylesheet (e.g. assets/css/main.scss) */
.publications {
  display: grid;
  row-gap: 2rem;
  margin-top: 1rem;
}

.pub-entry {
  padding-bottom: 1.5rem;
  border-bottom: 1px solid #eee;
}

.pub-entry .badge {
  display: inline-block;
  background: #4a148c;
  color: white;
  padding: 0.1em 0.6em;
  font-size: 0.75rem;
  border-radius: 3px;
  text-transform: uppercase;
  margin-bottom: 0.4rem;
}

.pub-entry h3 {
  margin: 0.2em 0;
  font-size: 1.1rem;
}

.pub-entry p {
  margin: 0.2em 0;
  color: #555;
}

.pub-entry .btn {
  display: inline-block;
  margin-top: 0.5rem;
  padding: 0.3em 0.8em;
  border: 1px solid #555;
  border-radius: 3px;
  font-size: 0.85rem;
  text-decoration: none;
  color: #555;
}

.pub-entry .btn:hover {
  background: #f5f5f5;
}
</style>

---
## Experience

### Cerebra | Applied AI Researcher
*Aug 2023 – Present*

- Developed a speech recognition system for Russian and Kazakh languages, integrating RAG and custom preprocessing techniques to reduce Word Error Rate (WER) by 20%; deployed in two hospitals and enhanced clinical efficiency through scalable inference on 60 hours of data using NVIDIA Riva
- Researched interpretability of stroke detection models with Grad-CAM++, providing generalized visual explanations for model decisions in medical imaging; augmented Latin corpus by 6000+ tokens for domain-specific vocabulary
- Designed and trained an AttentionUNet model for tumor segmentation, achieving a 72% F1 score in detecting intracerebral hemorrhage through a custom encoder-decoder architecture
- Led the research, development, and implementation of a multi-token prediction and shared trunk architecture for an auto-completion project aimed at supporting doctors with radiology documentation; spearheaded precise radiology scan modifications using multimodal vision-language understanding with the Qwen2-VL model

### Litigence | Applied AI Researcher
*May 2024 – Jul 2024*

- Engineered LangChain powered Knowledge Graph for 10,000+ patents for query answering and knowledge extraction
- Developed RAG search system to streamline patent retrieval across multiple documents, effectively utilizing UMAP to reduce high-dimensional embeddings and reduced query response latency by 85% compared to semantic search

### NKM Capital | Data Science in Residence
*Jun 2023 – Sep 2023*

- Devised a strategy for deal flow pipeline by analyzing early-stage YC startups and web scraping 1,500 M&A and IPO deals, identifying key patterns and early signals to enhance data-driven decision-making and support thesis development
- Engineered an algorithm to solve the rank aggregation problem for the portfolio company, resulting in an 8% improvement in F1 score accuracy across a multi-platform dataset (Google Reviews, Yelp, OpenTable)

---

## Skills

**Languages:** Python, R, MATLAB, NoSQL, SQL, HTML/CSS, Java

**Industry Knowledge:** Machine Learning, NLP, Computer Vision, Statistical Analysis, Knowledge Graphs, Neural Networks, CNN, RNN, Foundation Models, Generative AI, Data Pipeline Development, Deep Learning, Data Engineering, LLMs

**Technologies/Frameworks:** PyTorch, Git, TensorFlow, REST API, Pandas, AWS, NumPy, HuggingFace, ROS, JAX, CUDA


Outside of work, you’ll usually find me behind a camera lens, and training for another marathon.

<center>© 2025 Shyryn Ospanova. Powered by Jekyll and the Minimal Theme.</center>
