---
title: "Real-Time IMU-Based Motion Analysis System"
excerpt: "A wearable-style embedded system on an ARM Cortex-M4 that detects tremor, dyskinesia and Freezing of Gait in real time using an RTOS pipeline, on-device FFT and a custom BLE service."
collection: portfolio
order: 2
kind: "Embedded Systems"
org: "New York University"
period: "Mar 2026 – Jul 2026"
icon: "fa-microchip"
theme: "violet"
highlight: "Continuous 52 Hz sensing with on-device FFT and BLE result streaming"
stack: [ARM Cortex-M4, RTOS, CMSIS-DSP, I2C, BLE GATT]
---

<p class="project-meta"><span><i class="fas fa-building-columns"></i> New York University</span><span><i class="fas fa-user"></i> Embedded Systems Project</span><span><i class="fas fa-calendar"></i> Mar 2026 – Jul 2026</span></p>

## Overview

A real-time motion analysis system for movement-disorder symptoms. It runs entirely on a resource-constrained microcontroller, from raw sensor registers to wireless output.

## What I built

- **Register-level sensor driver.** An LSM6DSL IMU driver over **400 kHz I2C** on an ARM Cortex-M4, with configured sensor parameters and interrupt-driven acquisition for real-time **52 Hz** motion sensing.
- **Multi-threaded RTOS pipeline.** Priority scheduling and **double buffering** keep sensor acquisition separate from **CMSIS-DSP FFT** processing, so frequency-domain analysis runs continuously on limited hardware.
- **Stateful motion classification.** Detection of **tremor, dyskinesia and Freezing of Gait** that combines spectral analysis with motion-state transitions. Results are sent over a custom **BLE GATT** service.

## System at a glance

<div class="flow">
  <span>LSM6DSL IMU</span><i class="fas fa-arrow-right"></i>
  <span>I2C + IRQ driver</span><i class="fas fa-arrow-right"></i>
  <span>Double buffer</span><i class="fas fa-arrow-right"></i>
  <span>CMSIS-DSP FFT</span><i class="fas fa-arrow-right"></i>
  <span>State classifier</span><i class="fas fa-arrow-right"></i>
  <span>BLE GATT</span>
</div>
