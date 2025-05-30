---
layout: default
---
<nav class="section-nav">
  <a href="#projects">Projects</a> ·
  <a href="#pubs">Publications</a> ·
  <a href="#skills">Skills</a>
</nav>
<style>/* 1. Smooth scrolling for in‐page anchors */
html {
  scroll-behavior: smooth;
}

/* 2. Push the page down so content isn't hidden under our fixed bar */
body {
  padding-top: 3.5rem; /* match the nav’s height + any border */
}

/* 3. The fixed, full‐width nav */
.section-nav {
  position: fixed;
  top: 0; left: 0; right: 0;
  display: flex;
  justify-content: center;
  gap: 2rem;
  background: #ffffff;
  padding: 0.75rem 1rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
  border-bottom: 1px solid #eaeaea;
  z-index: 1000;
}

/* 4. Make each link’s whole padded area clickable */
.section-nav a {
  display: inline-block;
  padding: 0.4rem 0.8rem;
  color: #007acc;
  text-decoration: none;
  font-weight: 500;
  border-radius: 4px;
  transition: background-color 0.2s ease, color 0.2s ease;
}

/* 5. Hover + active states */
.section-nav a:hover {
  background-color: rgba(0, 122, 204, 0.1);
}

.section-nav a:active,
.section-nav a.active {
  background-color: rgba(0, 122, 204, 0.2);
  color: #005999;
}
/* Optional: Highlight the current section in nav as you scroll */
<script>
  document.addEventListener('DOMContentLoaded', () => {
    const navLinks = document.querySelectorAll('.section-nav a');
    const sections = Array.from(navLinks).map(a => document.querySelector(a.getAttribute('href')));

    const activateLink = () => {
      const scrollPos = window.scrollY + 80; // adjust offset to account for nav height
      sections.forEach((sec, i) => {
        if (sec.offsetTop <= scrollPos && sec.offsetTop + sec.offsetHeight > scrollPos) {
          navLinks.forEach(a => a.classList.remove('active'));
          navLinks[i].classList.add('active');
        }
      });
    };

    window.addEventListener('scroll', activateLink);
    activateLink();
  });
</script>
</style>



## Projects {#projects}

### Recurrent LidarNet
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

### Model Predictive Control
*Python, CVXPY, OSQP, ROS2, NumPy*  

Implemented a real-time MPC planner that linearizes & discretizes a kinematic bicycle model over a finite horizon to track spline waypoints with minimal tracking error, smooth control effort, and hard actuator limits. The QP minimizes:
- Deviation from reference (terminal & running weights)  
- Control magnitude  
- Inter-step control variations
- 
Visualization in simulation shows both the reference segment and MPC-predicted rollout.

<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/_u5AkwzfRfo"
  title="YouTube video player"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>

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
*Python, OpenCV, YOLO*

Produced the first public curriculum on Neural Networks and Computer Vision (OpenCV) in Russian with Kazakh subtitles for 500+ learners. Designed presentations and devised scripts for over 15 YouTube video-lessons with 7500+ views.
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
## Publications {#pubs}

<div class="publications">
  
<div class="pub-entry">
    <span class="badge">PLOS ONE</span>
    <h3>The impact of variance in carnitine palmitoyltransferase-1 expression on breast cancer prognosis is stratified by clinical and anthropometric factors</h3>
    <p>Ryan Liu, Shyryn Ospanova, Rachel J. Perry</p>
    <p><em>PLoS ONE 18(2): e0281252, published 3 February 2023</em></p>
    <p><a class="btn" href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0281252" target="_blank">View article</a></p>
  </div>
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
    <!-- Added simulation GIF below the IEEE paper entry -->
    <div style="margin-top: 1rem; text-align: center;">
      <img src="/assets/img/simulation.gif" alt="Simulation preview" style="max-width: 100%; height: auto; border: 1px solid #ccc;" />
    </div>
  </div>

</div>

<style>
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

## Skills {#skills}

- **Programming & DevOps:** Python, R, MATLAB, Java, SQL/NoSQL, HTML/CSS; Git, Docker, GitHub Actions, AWS (EC2/S3/Lambda), REST APIs  
- **Machine Learning & AI:** PyTorch, TensorFlow, JAX, Scikit-learn, Hugging Face; CNNs, RNNs/LSTMs, Transformer architectures, agent-based & reinforcement modeling  
- **Computer Vision & Robotics:** OpenCV, YOLO, SLAM, real-time 3D reconstruction, Attention-UNet segmentation; ROS2, CVXPY/OSQP for Model Predictive Control, LiDAR + IMU + camera fusion  
- **NLP & Knowledge Systems:** Clinical ASR pipelines, tokenization, Retrieval-Augmented Generation (RAG), LangChain, knowledge graphs, semantic search

---

> **Outside of work:** You’ll usually find me behind a camera lens or training for my next marathon.

<center>© 2025 Shyryn Ospanova. Powered by Jekyll and the Minimal Theme.</center>
