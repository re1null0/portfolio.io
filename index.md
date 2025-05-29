---
layout: default
---

# Shyryn Ospanova

## Applied AI Researcher

I am an Applied AI Researcher with expertise in machine learning, natural language processing, and computer vision. With a strong background in developing innovative AI solutions for healthcare and legal tech, I combine technical expertise with practical problem-solving skills.

## Experience

### Cerebra | Applied AI Researcher, Astana, Kazakhstan
*Aug 2023 – Present*

- Developed a speech recognition system for Russian and Kazakh languages, integrating RAG and custom preprocessing techniques to reduce Word Error Rate (WER) by 20%; deployed in two hospitals and enhanced clinical efficiency through scalable inference on 60 hours of data using NVIDIA Riva
- Researched interpretability of stroke detection models with Grad-CAM++, providing generalized visual explanations for model decisions in medical imaging; augmented Latin corpus by 6000+ tokens for domain-specific vocabulary
- Designed and trained an AttentionUNet model for tumor segmentation, achieving a 72% F1 score in detecting intracerebral hemorrhage through a custom encoder-decoder architecture
- Led the research, development, and implementation of a multi-token prediction and shared trunk architecture for an auto-completion project aimed at supporting doctors with radiology documentation; spearheaded precise radiology scan modifications using multimodal vision-language understanding with the Qwen2-VL model

### Litigence | Applied AI Researcher, Oslo, Norway
*May 2024 – Jul 2024*

- Engineered LangChain powered Knowledge Graph for 10,000+ patents for query answering and knowledge extraction
- Developed RAG search system to streamline patent retrieval across multiple documents, effectively utilizing UMAP to reduce high-dimensional embeddings and reduced query response latency by 85% compared to semantic search

### NKM Capital | Data Science in Residence, San Francisco, CA
*Jun 2023 – Sep 2023*

- Devised a strategy for deal flow pipeline by analyzing early-stage YC startups and web scraping 1,500 M&A and IPO deals, identifying key patterns and early signals to enhance data-driven decision-making and support thesis development
- Engineered an algorithm to solve the rank aggregation problem for the portfolio company, resulting in an 8% improvement in F1 score accuracy across a multi-platform dataset (Google Reviews, Yelp, OpenTable)

---

## Projects

### Recurrent LidarNet
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/re1null0)
*Python, PyTorch, CUDA, ROS2*

Extended 1D-CNN TinyLidarNet with a bidirectional LSTM + self-attention module, lifting lap-completion reliability from 30–78% to 100% on F1TENTH tracks and cutting average lap times by 11%. Quantized to TFLite INT8 (XNNPACK) and TensorRT FP16, achieving < 3 ms CPU and < 0.6 ms GPU inference while maintaining full generalization across novel tracks.
<div class="video-container">
  <video width="100%" controls>
    <source src="/assets/videos/rln" type="video/mp4">
    Your browser does not support the video tag.
  </video>
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

.video-container video {
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

---

## Research Experience

### Institute of Smart Systems and Artificial Intelligence | Research Intern, Astana, Kazakhstan
*Jun 2021 – Aug 2021*

- Simulated vaccination policies using agent-based modeling to identify the most effective strategies for reducing disease transmission; modeled sterilizing and effective immunization outcomes by adding 4 new SEIR states
- Published paper in IEEE titled "A Vaccination Simulator for COVID-19: Effective and Sterilizing Immunization Cases"

### Yale School of Medicine | Research Assistant, New Haven, CT
*Jul 2020 – Jun 2021*

- Developed analysis on lung cancer survivability with 94% accuracy; implemented a novel approach to incorporate quantitative and qualitative multivariate analysis using Python and TCGA on 20 Gigabytes PET/CT scans, leading to significant differentiation between lung squamous cell carcinoma and adenocarcinoma
- Published findings in Nature and PLOS One, focusing on differential immuno-metabolic crosstalk in lung cancer types and carnitine palmitoyltransferase-1 impact on breast cancer prognosis

---

## Skills

**Languages:** Python, R, MATLAB, NoSQL, SQL, HTML/CSS, Java

**Industry Knowledge:** Machine Learning, NLP, Computer Vision, Statistical Analysis, Knowledge Graphs, Neural Networks, CNN, RNN, Foundation Models, Generative AI, Data Pipeline Development, Deep Learning, Data Engineering, LLMs

**Technologies/Frameworks:** PyTorch, Git, TensorFlow, REST API, Pandas, AWS, NumPy, HuggingFace, ROS, JAX, CUDA

<center>© 2025 Shyryn Ospanova. Powered by Jekyll and the Minimal Theme.</center>
