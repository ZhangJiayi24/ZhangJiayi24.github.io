---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  dl {
    margin-bottom: 60px; /* 调整这个值以获得合适的间距 */
    clear: both;
  }

  /* 全局文本颜色 */
  body {
    color: #333; /* 主要文本颜色 */
    background-image: url('../images/bg.jpg'); /* 背景图片 */
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
  }

  /* 链接颜色 */
  a {
    color: #0066cc; /* 链接颜色 */
  }

  /* 作者名字颜色 */
  strong {
    color: #000; /* 作者名字颜色 */
  }

  /* 年份标题颜色 */
  .year-title {
    color: #666;
  }

  /* 会议标签样式 */
  .conference-label {
    position: absolute;
    top: 10px;
    left: -5px;
    background-color: #2c3e50;  /* 深蓝色背景 */
    color: white;  /* 白色文字 */
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 0.95em;
    font-weight: 600;
    letter-spacing: 0.5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    z-index: 1;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-style: italic;  /* 添加斜体 */
  }

  /* 鼠标悬停效果 */
  .conference-label:hover {
    background-color: #34495e;  /* 悬停时稍微变亮 */
    transition: background-color 0.2s ease;
  }

  dl dt img {
    width: 100%; /* 在移动端默认占满宽度 */
    aspect-ratio: 2/1; /* 设置宽高比为2:1，即高度为宽度的一半 */
    object-fit: cover; /* 确保图片不会被裁剪 */
    display: block;
    margin: 10px 10px 10px 0px; /* 适当的间距 */
    
    /* 添加美化效果 */
    border-radius: 8px; /* 让图片有轻微的圆角 */
    border: 2px solid #ddd; /* 添加淡灰色的边框 */
    box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2); /* 添加轻微阴影 */
    padding: 5px; /* 给图片一些内边距，让它不贴着边框 */
    background-color: #fff; /* 设置背景色，让图片更加干净 */
  }

  /* 在桌面端（宽度大于768px）时固定宽度 */
  @media screen and (min-width: 768px) {
    dl dt img {
      width: 350px;
    }
  }

  dl dt {
    position: relative;
  }

  hr {
    border: 1px solid #ebebeb; /* 调整分隔线的颜色和样式 */
    /* margin: 10px;  */
    clear: both; 
  }

  dl dd {
  margin-top: 5px; 
  margin-bottom: 5px;
}

  dl dd strong {
  font-weight: bold;
  color: black;
  }

  .co-first {
    color: red;
  }

  .down {
    transform: rotate(180deg);
  }

  /* 教育和工作经历卡片样式 */
  .experience-card, .education-card {
    display: flex;
    align-items: center;
    gap: 25px;
    margin-bottom: 30px;
    padding: 20px;
    background: #f8f9fa;
    border-radius: 12px;
    transition: all 0.3s ease;
    border: 1px solid #e9ecef;
  }

  .experience-card:hover, .education-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    border-color: #dee2e6;
  }

  .experience-info, .education-info {
    flex: 1;
  }

  .experience-logo, .education-logo {
    flex-shrink: 0;
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: white;
    border-radius: 10px;
    padding: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  }

  .experience-logo img, .education-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .experience-title, .education-title {
    font-size: 1.2em;
    margin-bottom: 8px;
    color: #2c3e50;
  }

  .experience-title a, .education-title a {
    color: #2c3e50;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .experience-title a:hover, .education-title a:hover {
    color: #3498db;
  }

  .experience-role, .education-role {
    color: #666;
    font-style: italic;
    margin-bottom: 5px;
  }

  .experience-topics, .education-topics {
    color: #666;
    font-style: italic;
  }

  .section-title {
    font-size: 1.8em;
    color: #2c3e50;
    margin: 40px 0 20px;
    padding-bottom: 10px;
    border-bottom: 2px solid #ecf0f1;
  }

  /* 奖学金和荣誉部分样式 */
  .honors-list {
    list-style: none;
    padding: 0;
  }

  .honors-list li {
    margin-bottom: 15px;
    padding: 15px 20px;
    background: #f8f9fa;
    border-radius: 8px;
    border-left: 4px solid #3498db;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .honors-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .honors-list li strong {
    color: #2c3e50;
  }

  .honors-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .honors-list li a:hover {
    color: #2980b9;
  }

  /* 服务部分样式 */
  .service-section {
    margin-bottom: 30px;
  }

  .service-section h3 {
    color: #2c3e50;
    font-size: 1.3em;
    margin: 25px 0 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #ecf0f1;
  }

  .service-list {
    list-style: none;
    padding: 0;
  }

  .service-list li {
    margin-bottom: 12px;
    padding: 12px 15px;
    background: #f8f9fa;
    border-radius: 6px;
    transition: transform 0.3s ease;
  }

  .service-list li:hover {
    transform: translateX(5px);
  }

  .service-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .service-list li a:hover {
    color: #2980b9;
  }
</style>

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>


My name is Jiayi Zhang (张珈译), a Mathematics and Applied Mathmatics Undergrad student at University of Nottingham Ningbo China ([UNNC]([https://www.ucla.edu/](https://www.nottingham.edu.cn/en/index.aspx))). 

I am open to any relavant research collaboration and internship. 🥳 Feel free to contact me via <a href="mailto:smyjz19@nottingham.edu.cn">Email</a> or <a href="https://ZhangJiayi24.github.io/images/Wechat.png">WeChat</a>.


<!-- Previously, I spent a wonderful summer at Emory University, supervised by [Wei Jin](https://scholar.google.com/citations?user=eWow24EAAAAJ&hl=en&oi=ao), [Carl Yang](https://scholar.google.com/citations?user=mOINlwcAAAAJ&hl=en&oi=ao) 
and collaborated with [B. Aditya Prakash](https://scholar.google.com/citations?user=C-NftTgAAAAJ). -->

<!--

<div style="text-align: left; margin: 20px 0;">
  <img src="../images/sign.png" alt="Signature" style="max-width: 150px; height: auto;">
</div>

Previously, I spent a wonderful summer at Emory University, supervised by [Wei Jin](https://scholar.google.com/citations?user=eWow24EAAAAJ&hl=en&oi=ao), [Carl Yang](https://scholar.google.com/citations?user=mOINlwcAAAAJ&hl=en&oi=ao) 
and collaborated with [B. Aditya Prakash](https://scholar.google.com/citations?user=C-NftTgAAAAJ).

<div style="text-align: left; margin: 20px 0;">
  <img src="../images/sign.png" alt="Signature" style="max-width: 150px; height: auto;">
</div>

<div style="background: linear-gradient(135deg, #f3f8ff, #e8f4fd); padding: 20px; border-radius: 10px; margin: 20px 0; border: 2px solid #1976d2; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1); position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: linear-gradient(135deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.3)); pointer-events: none;"></div>
  <p style="margin: 0; position: relative; z-index: 1;"> <strong style="color: red">🌟 📢 Seeking for Remote Intern/Assistant (RA)</strong><br>
We are looking for motivated research interns to work together! Almost every intern who worked with me has published papers at top conferences such as ICML, NeurIPS, ICLR and CVPR. If you are interested, please don't hesitate to contact me via <a href="mailto:gcwan03@ucla.edu">Email</a> or <a 
href="https://guanchengwan.github.io/images/wechat.png">WeChat</a>.
  </p>
</div>

-->



# 🔎 Research 
<!-- "All things are interconnected, this is the essence of nature."  -->

<!-- <dt style="text-align: center; margin: 0; padding: 0;"> -->
  <!-- <img src="../images/research.png" style="display: block; max-width: 700px; width: 100%; height: auto; margin: 0 auto;"> -->
<!-- </dt> -->

I am passionate about developing efficient and intelligent systems that connect decision, control, and real-world interaction. My current research interests focus on three key areas:

a) Robotics Manipulation: Perception-aware policy learning and generalizable control for physical interaction 

b) Control-oriented Reinforcement Learning: Offline or online methods for continuous control and real-world decision making

c) Large Model Inference Acceleration: Efficient architectures and optimization strategies for fast reasoning with foundation models


# 🔥 News

<div style="max-height: 350px; overflow-y: auto; padding: 20px; background: #f8f9fa; border-left: 4px solid #2c3e50; margin: 0px 0;">
<style>
  /* 为 Webkit 浏览器（Chrome, Safari, Edge）设置滚动条样式 */
  div::-webkit-scrollbar {
    width: 8px;
  }

  div::-webkit-scrollbar-track {
    background: #e9ecef;
    border-radius: 4px;
  }

  div::-webkit-scrollbar-thumb {
    background: #2c3e50;
    border-radius: 4px;
  }

  div::-webkit-scrollbar-thumb:hover {
    background: #1a252f;
  }

  /* 为 Firefox 设置滚动条样式 */
  div {
    scrollbar-width: thin;
    scrollbar-color: #2c3e50 #e9ecef;
  }
</style>
<ul style="list-style-type: none; padding-left: 0; margin: 0;">
  <li><em>2025.0:</em> 🎉 Great honor to have the opportunity to be a research assist at the <strong>IWIN-FINS lab</strong> at the <strong>Shanghai Jiao Tong University.</strong> </li>
  <li><em>2025.06:</em> 🎉 Our paper: Multi-Cali Anything was selected as an <strong class="co-first">Oral Presentation</strong> at <strong>IROS 2025</strong>. Thanks to all collaborators!</li>
  <li><em>2025.06:</em> 🎉 Our work: Spec-LLaVA was accepted by <strong>ICML 2025 TTODLer-FM workshop</strong>. See you in Vancouver.</li>
  <li><em>2025.05:</em> 🎉 We got Honorable Mention (Second Prize) in ICM 2025! Congrads and thanks to my teammates!</li>
  <li><em>2025.04:</em> 🎉 My personal academic homepage is now online.</li>
  <li><em>2025.03:</em> 🎉 Great honor to have the opportunity to be a research intern at the <strong>IoT lab</strong> at the <strong>University of Hong Kong.</strong> </li>
  <li><em>2025.03:</em> 🎉 Our work: SCANet was accepted by <strong>ICLR 2025 Tackling ClimateChange with Machine Learning Workshop</strong>. See you in Singapore.</li>
  <li><em>2025.01:</em> I completed two additional AI4S articles during the machine learning process.</li>
  <li><em>2025.01:</em> I participated in The Interdisciplinary Contest in Modeling (ICM).</li>
  <li><em>2024.12:</em> I participated in writing a paper for the first time and began studying machine learning.</li>
</ul>
</div>

<br/>




<!-- 

# 📝 Manuscripts

<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/MOTION.png">
<span class="conference-label">Under Review</span>
</dt>
  <dd><a href=""><strong>MOTION: Multi-Sculpt Evolutionary Coarsening for Federated Continual Graph Learning</strong></a></dd>
<dd>under review, 2025</dd>
</dl>

<hr>

<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/HYPERION.png">
<span class="conference-label">Under Review</span>
</dt>
  <dd><a href=""><strong>HYPERION: Fine-Grained Hypersphere Alignment for Robust Federated Graph Learning</strong></a></dd>
<dd>under review, 2025</dd>
</dl>

<hr>

<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/TRUST.png">
<span class="conference-label">Under Review</span>
</dt>
  <dd><a href=""><strong>Multi-order Orchestrated Curriculum Distillation for Model-Heterogeneous Federated Graph Learning</strong></a></dd>
<dd>under review, 2025</dd>
</dl>

<hr>

<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/OASIS.png">
<span class="conference-label">Under Review</span>
</dt>
  <dd><a href=""><strong>OASIS: One-Shot Federated Graph Learning via Wasserstein Assisted Knowledge Integration</strong></a></dd>
<dd>under review, 2025</dd>
</dl>

<hr> -->


# 📃 Selected Publications ([Full List](https://scholar.google.com/citations?hl=en&user=bLUpHDsAAAAJ))

**&dagger; Equal Contribution**   

<div style="text-align: left; margin: 20px 0; font-size: 1.5em; color: #666;">
2025 
</div>

<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/FedTGE.png">
<span class="conference-label">ICLR 2025</span>
</dt>
  <dd><a href="https://openreview.net/forum?id=5Jc7r5aqHJ"><strong>	
Energy-based Backdoor Defense Against Federated Graph Learning
</strong></a></dd>
<dd><strong><strong>Guancheng Wan</strong>&dagger;</strong>, Zitong Shi&dagger;, Wenke Huang&dagger;, Guibin Zhang, Dacheng Tao, Mang Ye</dd>
<dd> <strong class="co-first"><i>Oral Presentation (Top 1.8%)</i></strong> in International Conference on Learning Representations (<strong>ICLR</strong>), 2025</dd>
</dl>

<hr>


<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/GREAT.png">
<span class="conference-label">ICML 2025</span>
</dt>
  <dd><a href=""><strong>Rethink GraphODE Generalization within Coupled Dynamical System</strong></a></dd>
<dd><strong>Guancheng Wan</strong>, Zijie Huang, Wanjia Zhao, Xiao Luo, Yizhou Sun, Wei Wang</dd>
<dd>  <strong class="co-first"><i>Spotlight Presentation (Top 2.6%)</i></strong> in International Conference on Machine Learning (<strong>ICML</strong>), 2025</dd>
</dl>

<hr>


<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/LoRASculpt.png">
<span class="conference-label">CVPR 2025</span>
</dt>
  <dd><a href=""><strong>LoRASculpt: Sculpting LoRA for Harmonizing General and Specialized Knowledge in Multimodal Large Language Models</strong></a></dd>
  <dd>Jian Liang&dagger;, Wenke Huang&dagger;, <strong>Guancheng Wan&dagger;</strong> <span class="co-first">(co-first)</span>, Qu Yang, Mang Ye</dd>
  <dd><strong class="co-first"><i>Oral Presentation (Top 3.3%)</i></strong> in Conference on Computer Vision and Pattern Recognition (<strong>CVPR</strong>), 2025</dd>
</dl>

<hr>


<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/FedSPA.png">
<span class="conference-label">CVPR 2025</span>
</dt>
  <dd><a href=""><strong>FedSPA: Generalizable Federated Graph Learning under Homophily Heterogeneity</strong></a></dd>
  <dd>Zihan Tan&dagger;, <strong>Guancheng Wan&dagger;</strong> <span class="co-first">(co-first)</span>, Wenke Huang, Guibin Zhang, He Li, Carl Yang, Mang Ye</dd>
  <dd>Conference on Computer Vision and Pattern Recognition (<strong>CVPR</strong>), 2025</dd>
</dl>

<hr>


<dl>
  <dt><img align="left" width="100"
hspace="10" wspace="20" src="../images/EARTH.png">
<span class="conference-label">ICML 2025</span>
</dt>
  <dd><a href="https://arxiv.org/abs/2410.00049"><strong>Epidemiology-Aware Neural ODE with Continuous Disease Transmission Graph</strong></a></dd>
<dd><strong>Guancheng Wan</strong>, Zewen Liu, Xiaojun Shan, Max S.Y. Lau, B. Aditya Prakash, Wei Jin</dd>
<dd>International Conference on Machine Learning (<strong>ICML</strong>), 2025</dd>
</dl>


<hr>


<br>


# 🔬 Survey and Benchmark

- **Keeping Yourself is Important in Downstream Tuning Multimodal Large Language Model**

- **Protein Large Language Models: A Comprehensive Survey**

- **A Comprehensive Survey in LLM (-Agent) Full Stack Safety: Data, Training and Deployment**

- **From Web Search towards Agentic Deep ReSearch: Incentivizing Search with Reasoning Agents**

- **A Comprehensive Survey of Evaluating Multimodal Foundation Models: Hierarchical Perspective and Extensive Applications**

- **A Comprehensive Survey on Scientific Large Language Models in Physics**

- **FD-Bench: A Modular and Fair Benchmark for Data-driven Fluid Simulation**






# 🎡 Service

<div class="service-section">
  <h3>Program Chair</h3>
  <ul class="service-list">
    <li><a href="https://fedkdd.github.io/fedkdd2025/">FedKDD 2025 Workshop@KDD 2025</a></li>
  </ul>
</div>

<div class="service-section">
  <h3>Conference Committee Member</h3>
  <ul class="service-list">
    <li>Reviewer for NeurIPS'2025, EMNLP'2025</li>
  </ul>
</div>

<!--
<div class="service-section">
  <h3>Journal Reviewer</h3>
  <ul class="service-list">
    <li>IEEE TIFS, TIP, TKDE, TNNLS</li>
    <li>ACM TKDD</li>
    <li>Pattern Recognition (PR)</li>
    <li>Data-centric Machine Learning Research (DMLR)</li>
  </ul>
</div>
-->

<!-- - Reviewer for Data-centric Machine Learning Research (DMLR) -->


<br/>

# 🎖 Scholarships and Honors

- *2024.11* <a href="https://mp.weixin.qq.com/s/aS639YfEZLi2Y457L5XjUg">**Lei Jun Excellence Scholarship** </a>(**<u>雷军卓越奖学金</u>**) **~100k** (The **<u>Highest</u>** Scholarship at Wuhan University, **<u>Top-4</u>** among All Undergraduates, Award Rate ~ **0.01%**)  *Wuhan University*

- *2023.09* **National Scholarship** **(<u>Twice</u>)** (**<u>国家奖学金</u>**) (Award Rate: <strong>0.2% nation-wide</strong>) *Ministry of Education, China* 

- *2022.09* **National Scholarship** (**<u>国家奖学金</u>**) (Award Rate: <strong>0.2% nation-wide</strong>) *Ministry of Education, China* 

- *2025.03* <a href="https://mp.weixin.qq.com/s/1quPOGcxbMkfMFgkl8tFKQ">**Luo Jia Role model** </a>(榜样珞珈年度人物) (10 Students school-wide)  *Wuhan University*

- *2024.11* **InnoStar Undergraduate Innovation Achievement Award** (英诺大学生创新成果 特等奖) ~30k (**Only 2** Students school-wide) *Wuhan University*

- *2024.10* **Luojia Undergraduate Innovation Research Fund** (首批珞珈本科生研究基金) ~50k (4 Students department-wide)  *Wuhan University*

- *2024.06* **Lei Jun Computer Innovation and Development Fund** and  **Research Fund** (雷军创新发展基金、雷军研究基金) (3 Students department-wide)  *Wuhan University*

- *2024.06* <a href="https://scholarship2024.sensetime.com/cn/">**SenseTime Scholarship**</a> (商汤奖学金) ~20k (**25 Students nation-wide**) *SenseTime*

- *2024.04* <a href="https://mp.weixin.qq.com/s/zdx8hH8-g0FScgZvkYQRnw">**CS Pioneer**</a> (计科先锋年度人物) (10 Students department-wide)  *Wuhan University*

- *2023.10* **CCF (China Computer Federation) Elite Collegiate Award** (CCF优秀大学生) (102 Students nation-wide) *China Computer Federation*

- *2023.10* **Pacemaker to Merit Student** (三好学生标兵) (Award Rate ~ <strong>0.1%</strong>) *Wuhan University*


<br/>

# 📖 Education

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>2025.09 - Now</strong><br/>
      PhD, Computer Science, University of California, Los Angeles (UCLA)
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/UCLA.png" alt="UCLA Logo" />
  </div>
</div>

<!-- <div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>2021.09 - 2025.06</strong><br/>
      Bachelor, School of Computer Science, Wuhan University
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/WHU.jpeg" alt="Wuhan University Logo" />
  </div>
</div> -->


# 💼 Experience

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://www.princeton.edu/">Princeton University</a>
    </div>
    <div class="experience-role">Research Internship, 2025</div>
    <div class="experience-topics">Topics: AI for Science</div>
  </div>
  <div class="experience-logo">
    <img src="../images/princeton.png" alt="Princeton Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://sail.sea.com/">Sea AI Lab, Singapore</a>
    </div>
    <div class="experience-role">Internship, Associate member, 2025</div>
    <div class="experience-topics">Topics: (M)LLM, GUI Agent</div>
  </div>
  <div class="experience-logo">
    <img src="../images/sea.png" alt="Sea AI Lab Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://ucla-dm.github.io/DM_website/">UCLA Data Mining Lab</a> & <a href="http://web.cs.ucla.edu/~weiwang/">ScAI Lab</a>, University of California, Los Angeles
    </div>
    <div class="experience-role">Research Internship, 2024-2025</div>
    <div class="experience-topics">Topics: Ai4Science, Dynamic System, Graph Neural ODE</div>
  </div>
  <div class="experience-logo">
    <img src="../images/UCLA.png" alt="UCLA Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://www.cs.emory.edu/~wjin30/">Melody Lab</a>, Emory University
    </div>
    <div class="experience-role">Research Assistant, 2024</div>
    <div class="experience-topics">Topics: Ai4Science, Epidemiology, Graph Learning</div>
  </div>
  <div class="experience-logo">
    <img src="../images/emory.png" alt="Emory Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://adityalab.cc.gatech.edu/">Aditya Lab</a>, Georgia Institute of Technology
    </div>
    <div class="experience-role">Research Assistant, 2024</div>
    <div class="experience-topics">Topics: Ai4Science, Epidemiology, Graph Learning</div>
  </div>
  <div class="experience-logo">
    <img src="../images/gatech.png" alt="Georgia Tech Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://lucyinstitute.nd.edu/centers-and-labs/data-inference-analytics-and-learning-dial-lab/">DIAL Lab</a>, University of Notre Dame
    </div>
    <div class="experience-role">Research Internship, 2023</div>
    <div class="experience-topics">Topics: Inference Acceleration, Heterophilic Graph, Unsupervised Learning</div>
  </div>
  <div class="experience-logo">
    <img src="../images/ND.png" alt="Notre Dame Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://marswhu.github.io/">MARS lab</a>, Wuhan University
    </div>
    <div class="experience-role">Research Assistant, 2023-2025</div>
    <div class="experience-topics">Topics: Robustness, Backdoor Attack, Graph Learning, Domain Generalization, Federated Learning</div>
  </div>
  <div class="experience-logo">
    <img src="../images/WHU.jpeg" alt="WHU Logo" />
  </div>
</div>


<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://sigma.whu.edu.cn/">SIGMA lab</a>, Wuhan University
    </div>
    <div class="experience-role">Research Assistant, 2023-2025</div>
    <div class="experience-topics">Topics: Robustness, Backdoor Attack, Graph Learning, Domain Generalization, Federated Learning</div>
  </div>
  <div class="experience-logo">
    <img src="../images/sigma.png" alt="WHU Logo" />
  </div>
</div>


<dl><a href="https://clustrmaps.com/site/1bxa7" title="Visit tracker"><img src="//clustrmaps.com/map_v2.png?cl=080808&w=400&t=n&d=3d-gAqSb6Wx-DoL_BIvviv0g9ivHnOPl9-3M98ywjqw&co=ffffff&ct=808080" /></a></dl>




# 🏀 Miscellaneous

<details>
  <summary><strong>Talks and Shares</strong></summary>
<dd><a href="https://www.bilibili.com/video/BV1gZ42177VL/?spm_id_from=333.337.search-card.all.click&vd_source=0b7a3cc3d3ec288abaca83b9a7e036af"><strong>泛化图学习与本科生科研经历分享</strong></a></dd>




</details>


<details>
  <summary><strong>Undergraduate research resource and enrollment process</strong></summary>

<dd><a href="https://zxeupbuzh9y.feishu.cn/docx/ZDEsdpZtPosRWOxcBnkcF8Hknkd"><strong>Link</strong></a></dd>


</details>



<details>
  <summary><strong>Poems that inspire me</strong></summary>
  <dd><strong>白鹭立雪，愚者看鹭，聪者观雪，智者见白</strong> —— A white egret stands in the snow. The foolish see only the egret, the wise observe the snow, and the enlightened perceive the whiteness.</dd>
  <dd><strong>世界不黑也不白, 而是一道精致的灰</strong> —— The world is neither black nor white, but a delicate shade of gray. </dd>
    <dd><strong>风吹到哪页，读哪页</strong> —— The wind blows to which page, read which page.. </dd>
</details>




<br>

<br>

<br>

<br>
