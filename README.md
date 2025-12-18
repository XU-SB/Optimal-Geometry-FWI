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

This repository is organized primarily around a set of Jupyter notebooks.
Each notebook corresponds to a specific modeling or geometry test case used in FWI geometry evaluation.

#### FWI_Model_More_source.ipynb
FWI modeling test with an increased number of seismic sources, used to study the influence of source count on imaging results.

### FWI_Model_Opt1a.ipynb
FWI geometry optimization test case labeled Opt1a.

### FWI_Model_Opt1b.ipynb
FWI geometry optimization test case labeled Opt1b.

### FWI_Model_Opt1c.ipynb
FWI geometry optimization test case labeled Opt1c.

### Modeling_Model_surface.ipynb
Forward seismic modeling for surface acquisition geometry.

### Modeling_Model_VSP.ipynb
Forward seismic modeling for VSP-style acquisition geometry.

Each notebook is designed to be run independently and used for controlled comparison of different acquisition geometries and modeling setups.

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
