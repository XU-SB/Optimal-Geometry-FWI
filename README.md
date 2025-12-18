Optimal-Geometry-FWI

Optimal-Geometry-FWI is a Python-based research code for optimal acquisition geometry design in Full Waveform Inversion (FWI). The package is developed for geometry evaluation and survey design in both land and marine seismic acquisition, with emphasis on physics-based imaging capability rather than inversion algorithm development.

The code provides a controlled framework to study how source窶途eceiver layout, aperture, and deployment style influence FWI imaging performance. It supports surface seismic, VSP-style, and hybrid geometries, and is applicable to baseline and time-lapse (4D) monitoring problems.

---

Scope

This repository is intended for survey design and feasibility studies.

Primary objectives:
- Quantify geometry-controlled imaging capability in FWI
- Compare land and marine acquisition geometries
- Evaluate source窶途eceiver aperture and spacing effects
- Identify optimal geometries under practical constraints
- Provide reproducible and quantitative geometry-ranking metrics

---

Key Features

- Parameterized source and receiver geometry definition
- Acoustic and elastic forward modeling support
- Conventional FWI and double-difference FWI (DD-FWI)
- Imaging-map construction for geometry evaluation
- Quantitative metrics such as lateral imaging distance and image stability
- Modular structure for systematic geometry sweeps

---

Installation

Clone the repository:

git clone https://github.com/XU-SB/Optimal-Geometry-FWI.git

The code is developed and tested on Linux systems.
Use of a virtual environment or Conda environment is recommended.

---

Dependencies

Core dependencies:
- numpy
- scipy
- matplotlib
- pandas
- pyseis

Optional dependencies:
- jupyterlab
- nbformat
- papermill
- lasio

---

GPU Requirements

This package is designed for GPU-accelerated computation.

- At least one NVIDIA GPU with CUDA support is required for FWI
- Elastic FWI and large geometry sweeps benefit from multiple GPUs
- CPU-only execution is suitable only for small forward-modeling tests

---

Intended Use

This code is intended for research, feasibility analysis, and methodology development in seismic survey design.
It is not a production processing system and does not include field data.

---

Contact

Developer: Xu Shibo
Email: xushibo11@gmail.com
