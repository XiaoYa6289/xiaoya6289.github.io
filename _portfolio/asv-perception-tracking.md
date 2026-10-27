---
title: "ASV Perception & Temporal Tracking"
excerpt: "A perception and tracking pipeline for autonomous surface vessels that fuses YOLO detection, eWaSR segmentation and an Unscented Kalman Filter to keep track of targets in dynamic maritime scenes."
collection: portfolio
order: 1
kind: "Research"
org: "CREO Lab, NYU"
period: "Fall 2026"
icon: "fa-ship"
theme: "ocean"
highlight: "153 / 155 visible observations correctly assigned, only 2 identity switches"
stack: [YOLO, eWaSR, UKF, RANSAC, Python]
---

<p class="project-meta"><span><i class="fas fa-building-columns"></i> Control, Robotics, and Embodied Intelligence (CREO) Lab, NYU</span><span><i class="fas fa-user"></i> Graduate Researcher</span><span><i class="fas fa-calendar"></i> Fall 2026</span></p>

## Overview

Autonomous surface vessels (ASVs) have to see and follow other objects on the water while the camera pitches and rolls with the waves, detections flicker, and targets drift in and out of view. I built a perception and temporal tracking pipeline that turns noisy per-frame detections into stable, persistent target tracks.

## What I built

- **Detection, segmentation and state estimation.** YOLO-based object detection, eWaSR water segmentation and **Unscented Kalman Filter (UKF)** state estimation, combined into one tracking pipeline for changing maritime conditions.
- **Monocular range and bearing.** Camera timestamps aligned with vehicle telemetry, plus **RANSAC-based horizon estimation** to correct for camera pitch and roll, so range and bearing can be estimated from a single camera.
- **Robust data association.** Dual-confidence association and soft continuity costs that handle low-confidence detections, spatial jumps and class mismatches. Diagnostic visualizations help isolate where association fails.

## Results

<div class="result-row">
  <div class="result"><span>500+</span>confirmed track updates evaluated</div>
  <div class="result"><span>153 / 155</span>visible observations correctly assigned</div>
  <div class="result"><span>2</span>identity switches in proxy evaluation</div>
  <div class="result"><span>300</span>hand-labeled ground-truth frames used for validation</div>
</div>
