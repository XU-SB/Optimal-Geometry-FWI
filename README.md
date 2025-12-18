# Optimal-Geometry-FWI

**Optimal-Geometry-FWI** is a **Python-based** source code package developed by **Dr. Xu Shibo** from **ENEOS Xplora**. It provides a modular framework for **optimal acquisition geometry design** in **Full Waveform Inversion (FWI)**, targeting both **land and marine seismic surveys**.

The package focuses on quantifying how **source-receiver geometry controls imaging capability** in FWI, rather than on inversion algorithm development. By combining forward modeling, inversion, and quantitative imaging metrics, users can systematically evaluate survey designs, compare acquisition scenarios, and identify optimal geometries under practical constraints.

The toolkit supports surface seismic, VSP-style, and hybrid acquisition configurations, and is applicable to baseline and time-lapse (4D) monitoring problems, including CCS-related feasibility studies. The code is organized for flexibility and extensibility, enabling geometry sensitivity analysis, aperture studies, and imaging-map construction using reproducible synthetic experiments.

---

## Installation

To install **Optimal-Geometry-FWI**, first clone the repository:

git clone https://github.com/XU-SB/Optimal-Geometry-FWI.git

The package is designed to run on **Linux systems**.

For full functionality, it is recommended to use **JupyterLab** within a **virtual environment**.

---

## Required Modules

Core dependencies:

- pyseis
- numpy
- matplotlib
- pandas
- scipy

Optional (but useful) modules:

- papermill (for batch or parallel execution)
- lasio (for well log input)
- nbformat (for notebook handling)

---

## GPU Requirements

This package is designed for **GPU-based computation**.

At least one **NVIDIA GPU** with CUDA support is required to run FWI.  
For elastic FWI and large geometry sweeps, **multiple GPUs** are recommended.

---

## Package Overview

The package is organized into several functional modules, each targeting a specific aspect of geometry design and evaluation:

### Module 1: Forward Modeling

Acoustic and elastic forward modeling for land and marine survey configurations, including surface and VSP-style geometries.

### Module 2: Geometry Definition

Parameterization of source and receiver layouts, including spacing, aperture, and deployment type.

### Module 3: Geometry-Based Tests

Systematic evaluation of different acquisition geometries using conventional FWI and double-difference FWI (DD-FWI).

### Module 4: Sensitivity and Feasibility Analysis

Assessment of geometry robustness under:
- Aperture limitation
- Source-receiver spacing variation
- Initial model uncertainty
- Noise contamination

### Module 5: Imaging Map Generation

Construction of imaging maps and quantitative metrics, such as lateral imaging distance and image stability, for geometry ranking.

---

## Intended Use

This code is intended for **research, feasibility analysis, and survey design studies**.  
It is not a production processing system and does not include proprietary field data.

---

## Contact

For questions, issues, or contributions, please contact:

Xu Shibo  
xushibo11@gmail.com  
xu.shibo@eneos.com
