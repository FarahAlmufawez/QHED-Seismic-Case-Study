# QHED-Seismic-Case-Study

## Overview

This repository contains a case study investigating the application of **Quantum Hadamard Edge Detection (QHED)** to seismic image interpretation.

The project compares a quantum-inspired edge detection approach with a classical Sobel edge detector using synthetic seismic benchmark images. The objective is to explore whether quantum image processing techniques can identify geological-style boundaries relevant to seismic interpretation.

This work was completed as part of **PHY5003 Quantum Software** at **La Trobe University**.

---

## Project Objectives

* Investigate the principles of Quantum Hadamard Edge Detection (QHED).
* Apply QHED to synthetic seismic benchmark images.
* Compare QHED with a classical Sobel edge detector.
* Evaluate edge detection performance using quantitative metrics.
* Examine the scalability and resource requirements of QHED.
* Assess the potential relevance of quantum image processing to future seismic workflows.

---

## Benchmark Images

Two synthetic benchmark images are used:

### Single Boundary

A simple seismic-style image containing a single horizontal interface between two regions of different intensity.

### Checkerboard

A more challenging benchmark containing multiple horizontal and vertical boundaries distributed throughout the image.

These benchmarks provide controlled test cases where the true edge locations are known.

---

## Methods

### Classical Baseline

* Sobel Edge Detector

### Quantum Approach

* Amplitude Encoding
* Quantum Hadamard Edge Detection (QHED)
* Qiskit Aer Simulation
* Row-wise image processing

---

## Evaluation Metrics

The following metrics are used to compare the results:

* Structural Similarity Index (SSIM)
* Visual comparison of detected edge maps

---

## Repository Contents

```text
QHED-Seismic-Case-Study/
│
├── QHED_Seismic_Case_Study.ipynb
├── figures/
├── README.md
├── requirements.txt
└── report/
```

---

## Key Findings

* QHED successfully identified the major boundaries present in the benchmark images.
* The algorithm recovered the principal structural features detected by the Sobel operator.
* QHED produced thin, well-localised edge responses.
* No practical quantum advantage was demonstrated in this study.
* Current limitations are primarily related to quantum hardware and image state preparation.

---

## Requirements

Python 3.10+

Main packages:

```bash
numpy
matplotlib
qiskit
qiskit-aer
scipy
scikit-image
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Author

**Farah Almufawez**
Master of Quantum Information Technology
La Trobe University

---

## Disclaimer

This project is intended as a proof-of-concept academic case study. The implementation is designed to explore the potential of quantum image processing for seismic interpretation and should not be considered a production-ready seismic processing workflow.
