---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="cv-download">
  <div>
    <strong>Curriculum Vitae</strong>
    <span>Last updated October 2026</span>
  </div>
  <a class="pill-btn pill-btn--solid" href="{{ '/files/Xiaoya_Li_CV.pdf' | relative_url }}"><i class="fas fa-download"></i> Download PDF</a>
</div>

<h2 class="section-title"><i class="fas fa-graduation-cap"></i> Education</h2>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>New York University</h3><span>Brooklyn, NY</span></div>
  <div class="cv-entry__sub"><em>M.S. in Computer Engineering</em><span>Expected May 2027</span></div>
  <p>GPA: 4.0/4.0</p>
</div>
<div class="cv-entry">
  <div class="cv-entry__head"><h3>Anhui University</h3><span>Hefei, China</span></div>
  <div class="cv-entry__sub"><em>B.S. in Internet Banking</em><span>June 2025</span></div>
  <p>GPA: 3.64/4.0</p>
</div>
<p class="cv-note"><strong>Relevant coursework:</strong> Optimal Transport, Embedded Systems, Computer System Architecture, Big Data Analysis and Data Mining, Machine Learning, Python Programming</p>

<h2 class="section-title"><i class="fas fa-flask"></i> Research Experience</h2>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>CREO Lab (Control, Robotics, and Embodied Intelligence)</h3><span>New York University</span></div>
  <div class="cv-entry__sub"><em>Graduate Researcher, ASV Perception and Tracking</em><span>Fall 2026</span></div>
  <ul>
    <li>Developed an ASV perception and temporal tracking pipeline that combines YOLO-based detection, eWaSR segmentation and Unscented Kalman Filter (UKF) state estimation to track targets reliably in changing maritime conditions.</li>
    <li>Aligned camera timestamps with vehicle telemetry and added RANSAC-based horizon estimation to correct for camera pitch and roll, enabling monocular range and bearing estimation.</li>
    <li>Evaluated track continuity across 500+ confirmed updates. Designed dual-confidence association and soft continuity costs to handle low-confidence detections, spatial jumps and class mismatches, and built diagnostic visualizations to isolate data-association failures.</li>
    <li>Correctly assigned 153 of 155 visible target observations over time, with only 2 identity switches in proxy evaluation. Validated track consistency against a hand-labeled 300-frame ground-truth reference.</li>
  </ul>
</div>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>Real-Time IMU-Based Motion Analysis System</h3><span>New York University</span></div>
  <div class="cv-entry__sub"><em>Embedded Systems Project</em><span>Mar 2026 – Jul 2026</span></div>
  <ul>
    <li>Implemented a register-level LSM6DSL IMU driver over 400 kHz I2C on an ARM Cortex-M4, configuring sensor parameters and interrupt-driven acquisition for real-time 52 Hz motion sensing.</li>
    <li>Designed a multi-threaded RTOS pipeline with priority scheduling and double buffering that keeps sensor acquisition separate from CMSIS-DSP FFT processing, enabling continuous frequency-domain analysis on resource-constrained hardware.</li>
    <li>Developed a stateful motion-classification pipeline for tremor, dyskinesia and Freezing of Gait detection that combines spectral analysis with motion-state transitions, and sends results wirelessly through a custom BLE GATT service.</li>
  </ul>
</div>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>Reinforcement Learning-Based Intelligent Energy Optimization</h3><span></span></div>
  <div class="cv-entry__sub"><em>Independent Research Project</em><span>Sep 2025 – Dec 2025</span></div>
  <ul>
    <li>Formulated building HVAC control as a Markov Decision Process with defined state, action and reward spaces, and built an EnergyPlus simulation environment from historical operating data.</li>
    <li>Trained and compared PPO, DDPG and Q-learning agents over 1,000+ simulation episodes. The agents adapted temperature control to indoor and outdoor conditions and reduced simulated energy consumption by 20%.</li>
  </ul>
</div>

<h2 class="section-title"><i class="fas fa-briefcase"></i> Professional Experience</h2>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>Bolan Intelligent Technology Co., Ltd.</h3><span>Shenzhen, China</span></div>
  <div class="cv-entry__sub"><em>AI Strategy Intern</em><span>May 2026 – Aug 2026</span></div>
  <ul>
    <li>Built and evaluated AI-agent workflows by turning operational requirements into structured prompts, workflow logic and evaluation criteria for AI-assisted automation.</li>
    <li>Piloted LLM-powered customer-feedback analysis and recurring reporting workflows. Worked with operations teams to refine agent behavior, contributing to a 1.6% improvement in operational accuracy.</li>
  </ul>
</div>

<div class="cv-entry">
  <div class="cv-entry__head"><h3>Financial China Information &amp; Technology Co., Ltd.</h3><span>Shanghai, China</span></div>
  <div class="cv-entry__sub"><em>Machine Learning Intern</em><span>Feb 2025 – Aug 2025</span></div>
  <ul>
    <li>Built an XGBoost user-interest prediction model and improved its F1 score by 15% through feature and model tuning with grid-search optimization.</li>
    <li>Developed LightGBM-based recommendation logic and validated the production system with A/B testing, increasing conversion rate by 18% and average order value by 10%.</li>
  </ul>
</div>

<h2 class="section-title"><i class="fas fa-toolbox"></i> Languages &amp; Skills</h2>

<div class="skills">
  <div class="skills__row"><span class="skills__label">Programming</span>
    <span class="chip">Python</span><span class="chip">SQL</span><span class="chip">Java</span></div>
  <div class="skills__row"><span class="skills__label">Embedded &amp; Systems</span>
    <span class="chip">STM32</span><span class="chip">Mbed OS</span><span class="chip">RTOS</span><span class="chip">CMSIS-DSP</span><span class="chip">I2C</span><span class="chip">BLE GATT</span><span class="chip">PlatformIO</span></div>
  <div class="skills__row"><span class="skills__label">AI / ML</span>
    <span class="chip">PyTorch</span><span class="chip">TensorFlow</span><span class="chip">XGBoost</span><span class="chip">LightGBM</span><span class="chip">Reinforcement Learning</span><span class="chip">LLM / AI-Agent Workflows</span></div>
</div>
