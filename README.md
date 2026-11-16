# EarMotion: Wearable In-Ear EEG & Facial EMG Emotion Recognition System

## Overview
**EarMotion** (developed under the *BrainSense* project at Johns Hopkins University) is a non-invasive, wearable biosensing system designed to capture neurological and facial neuromuscular responses for continuous emotion recognition. 

Conventional laboratory-grade EEG setups are bulky and impractical for everyday affective monitoring, while single-modality wearables often lack physiological specificity. EarMotion addresses this by integrating **in-ear EEG electrodes** with **facial EMG sensors** into a compact, wearable form factor, pairing custom low-noise analog acquisition hardware with signal processing pipelines to decode emotional states in real time.

### Recognition & Funding
* **JHU Design Day:** Selected via faculty nomination for presentation at the Johns Hopkins University Whiting School of Engineering Design Day.
* **JHU Ignite Fund:** Awarded **$1,000** in competitive project funding to support hardware prototyping and validation.

---

## System Architecture

### 1. Multimodal Sensing & Custom Analog Front-End (AFE)
* **In-Ear EEG & Facial EMG Acquisition:** Captures microvolt-level neural oscillations from the ear canal alongside subtle facial muscle activation patterns associated with affective responses.
* **Analog Amplification & Filtering:** Independently designed, built, and bench-validated multi-stage analog front-end circuits—including high-CMRR instrumentation amplification, active bandpass filtering, and baseline drift suppression—to isolate clean physiological signals from motion and power-line interference.

### 2. Biosignal Processing & Feature Extraction
* **Noise & Artifact Mitigation:** Digital notch and bandpass filtering pipelines implemented in **Python** and **MATLAB** to attenuate eye-blink, jaw-clench, and motion artifacts.
* **Multimodal Feature Extraction:** Extracts time-domain EMG amplitude/burst metrics and frequency-band EEG spectral power features for affective state classification.

### 3. Visualization & Real-Time Monitoring
* Provides live multi-channel waveform display and real-time emotional state inference feedback during experimental recording sessions.

---

## Repository Structure
```text
EarMotion/
├── visualization/      # Live biosignal display and demo interface files
└── README.md
