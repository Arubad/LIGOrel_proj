# Gravitational-Wave Data Analysis Portfolio

This repository showcases my practical skills in gravitational-wave (GW) data analysis, developed as a portfolio for a research internship application with the LIGO-India collaboration at IUCAA.

The work contained in this repository demonstrates an end-to-end understanding of the foundational techniques used by LIGO-Virgo-KAGRA (LVK) scientists to detect signals and characterize detector noise using real, publicly available data.

---

## Projects Overview

The core of this portfolio is the `IUCAA_LIGO.ipynb` Jupyter Notebook, which contains two distinct projects. Each project is documented with conceptual explanations alongside the Python code.

### 📈 Project 1: Finding a Chirp — A Matched-Filter Search

This project implements the **matched filtering algorithm** to successfully detect the GW150914 signal in public data from the LIGO Hanford (H1) detector. It demonstrates the complete, fundamental analysis chain:
* **Data Conditioning**: Applying high-pass filters and resampling the raw detector strain data to prepare it for analysis.
* **Noise Characterization**: Estimating the detector's noise profile by calculating its Power Spectral Density (PSD) using Welch's method.
* **Template Waveform Generation**: Creating a theoretical "template" waveform from the parameters of a binary black hole merger.
* **Signal Detection**: Correlating the template with the data to produce a Signal-to-Noise Ratio (SNR) time-series and identifying the prominent peak corresponding to the GW150914 event.

---

### 🎧 Project 2: Detector Noise Forensics

This project analyzes the noise characteristics of the LIGO Livingston (L1) detector, a critical step in any real-world GW analysis. This demonstrates the ability to perform essential data quality assessments.
* **Amplitude Spectral Density (ASD)**: Generating an ASD plot to visualize the detector's average sensitivity and identify persistent instrumental noise, such as the 60 Hz electrical power line harmonics.
* **Time-Frequency Analysis**: Creating a spectrogram to visualize how the detector's noise content changes over time, identifying transient noise "glitches" and the non-stationary nature of the data.

---

## Skills and Libraries Demonstrated

This portfolio demonstrates proficiency in the following areas:

* **Languages**: Python
* **Core Libraries**:
    * **PyCBC**: The primary toolkit for GW signal processing, used for matched filtering and waveform generation.
    * **GWpy**: A high-level package for handling and visualizing gravitational-wave time-series data.
* **Key Concepts**:
    * Time-Series Analysis
    * Signal Processing (Filtering, Resampling, PSD Estimation)
    * Matched Filtering & Cross-Correlation
    * Data Visualization (Matplotlib/PyLab)
    * Detector Characterization & Noise Analysis

---

## How to Run This Project

To run the notebook yourself, you can open it in Google Colab or set up a local environment with the following dependencies installed:

```bash
pip install gwpy pycbc ligo-common
```
The first code cell in the notebook handles these installations automatically.
