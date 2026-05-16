# RadarFocusNet
Official PyTorch implementation of the core RadarFocusNet architecture and the FCT-Mix module for mmWave radar gesture recognition.
## 🔒 Data & Code Availability Disclaimer

* **Raw Radar Datasets:** Due to strict non-disclosure agreements (NDA) associated with the ongoing commercial project and ethical/privacy regulations regarding human volunteer data, the raw radar reflections cannot be made publicly available.
* **Academic Open-Source Commitment:** To ensure rigorous methodological reproducibility and facilitate community research, we open-source the complete, unmodified core deep learning model architecture definitions and forward propagation routines in this repository.

---

## 📢 News & Status

* **[2026/05]** 🚀 **The core implementation code is currently being cleaned up and anonymized for open-source release. It will be fully uploaded very soon! Stay tuned and welcome to Star this repository.**

---

## 📌 About

To address the fundamental flaw in existing mmWave radar gesture recognition methods—where traditional models (like CNNs or Transformers) treat radar spectrograms as ordinary RGB images and neglect their inherent physical frequency properties—this project introduces **RadarFocusNet**.

* **Dual-Stream Intermediate Fusion:** It independently processes multi-modal spectrograms (Doppler-Time Maps and Range-Time Maps), achieving deeply aligned spatio-temporal integration at an abstract feature level to overcome the informational limitations of single-source inputs.
* **Fourier-Domain Dynamic Convolution Mix (FCT-Mix):** Our core physics-driven innovation. It transforms intermediate features into the frequency domain to dynamically identify high-energy micro-motion components. By utilizing these spectral priors to generate spatially-varying dynamic convolutional kernels, it explicitly forces the network to shift from merely "recognizing superficial visual patterns" to truly "understanding the physical essence of radar signals."
