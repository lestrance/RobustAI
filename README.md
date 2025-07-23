# 📄 Validating the Adversarial Robustness of Hand-Crafted Features and Their Role in Defending Adversarial Examples

**IEEE Access 2025 (Under Review)**  
📅 Submitted: 1st July 2025  
🧠 Authors: Shuohan Xue, Charith Abhayaratne  
📬 [sxue6@sheffield.ac.uk](mailto:sxue6@sheffield.ac.uk)  
🔗 GitHub Repository: https://github.com/lestrance/RobustAI

---

## ⚠️ NOTICE – PAPER UNDER REVIEW

> 📢 **This repository has been made publicly available to support the peer-review process of our manuscript currently under review at _IEEE Access_ (submitted on 1st July 2025).**  
>  
> 🧪 The code, data, and results presented here are provided to help reviewers verify experimental reproducibility and assess technical contributions.  
>  
> 📌 **If you are a researcher or practitioner using this repository beyond peer review**, we kindly ask that you **cite our paper upon its formal acceptance and publication**.

---

## 📚 Overview

This repository contains the **official MATLAB R2024b implementation** of our IEEE Access 2025 paper.  
We introduce two novel defence mechanisms against adversarial examples:

- ✅ **Adversarial Awareness Score (AAS)** – a scalar metric that detects adversarial inputs using robust Wavelet Scattering Network (WSN) features.
- ✅ **AAS-guided Jacobian Regularisation** – a dynamic model regularisation strategy that improves adversarial robustness without degrading clean performance.

All experiments are implemented in MATLAB R2024b and validated on subsets of the ImageNet dataset.

---

## 📁 Repository Contents

This repository contains three self-contained MATLAB Live Scripts that include all necessary code, functions, and implementations:

```
RobustAI/
├── 📄 Experiment_01.mlx    # Complete implementation of WSN vs DNN feature robustness analysis
│                           # Includes: WSN feature extraction, adversarial attack generation.
│                           # robustness metrics calculation, and comparative visualisations
│
├── 📄 Experiment_02.mlx    # Full AAS calculation and evaluation pipeline  
│                           # Includes: AAS computation algorithms, detection threshold optimisation,
│                           # ROC analysis, and performance benchmarking against baselines
│
├── 📄 Experiment_03.mlx    # AAS-guided Jacobian Regularisation training framework
│                           # Includes: Dynamic regularisation implementation, model training loops.
│                           # adversarial robustness evaluation, and clean accuracy preservation
│
└── 📄 README.md           # This documentation file
```

**📋 Live Script Features:**
- **Self-contained**: Each `.mlx` file contains all required functions and implementations
- **Interactive**: Rich text explanations, live code execution, and inline visualisations  
- **Reproducible**: Fixed random seeds and documented parameters for consistent results
- **Educational**: Step-by-step explanations of algorithms and methodologies



## 🧪 Reproducing Experiments (Live Scripts)

We provide three MATLAB Live Scripts that reproduce the core experiments described in the paper. These scripts are self-contained and can be run interactively in MATLAB R2024b.

| Experiment | Description | Script |
|-----------|-------------|--------|
| **1** | Compare adversarial robustness of WSN and DNN features | `Experiment_01.mlx` |
| **2** | Calculate and evaluate the Adversarial Awareness Score (AAS) | `Experiment_02.mlx` |
| **3** | Retrain model with AAS-guided Jacobian Regularisation | `Experiment_03.mlx` |

> ✅ Tested with **MATLAB R2024b**  
> 📦 Required Toolboxes: *Deep Learning Toolbox*, *Wavelet Toolbox*, *Statistics and Machine Learning Toolbox*

---

## ⚙️ Setup Instructions

1. Clone this repository:
    ```bash
    git clone https://github.com/lestrance/RobustAI.git
    cd RobustAI
    ```

2. Launch MATLAB R2024b and set the working directory:
    ```matlab
    run('code/config/params.m'); % Sets up paths and global parameters
    ```

3. Run the Live Scripts in `notebooks/` to reproduce results.

---

## 📎 Citation

If our paper is officially accepted, please cite it as:

@article{xue2025aas,
  title={Validating the Adversarial Robustness of Hand-Crafted Features and Their Role in Defending Adversarial Examples},
  author={Xue, Shuohan and Abhayaratne, Charith},
  journal={IEEE Access},
  year={2025}
}


## Contact

For questions or collaborations, feel free to contact:

[Shuohan Xue](https://ieeexplore.ieee.org/author/37088931505) — sxue6@sheffield.ac.uk  
[Dr.Charith Abhayaratne](https://sheffield.ac.uk/eee/people/academic-staff/charith-abhayaratne) — c.abhayaratne@sheffield.ac.uk

## Author's Biography

Shuohan Xue received the B.E. degree in Mechatronics Engineering from the North University of China, Shanxi, China, in 2015, and the M.Sc. degree in Electronic and Electrical Engineering from the University of Sheffield, U.K., in 2019. He recently completed his Ph.D. in the Department of Electronic and Electrical Engineering at the University of Sheffield in 2024. His research focuses on interpretable and trustworthy deep learning, with particular interest in real-world scenarios such as human-level image recognition, medical imaging, and autonomous vehicles.

<img src="Images/xue.jpg" width="150" height="230">

Charith Abhayaratne(M’98) received the B.E. degree in electrical and electronic engineering from The University of Adelaide, Australia, in 1998, and the Ph.D. degree in electronic and electrical engineering from the University of Bath, U.K., in 2002. He was a recipient of the European Research Consortium for Informatics and Mathematics (ERCIM) Post-Doctoral Fellowship (2002-2004) to carry out research at the Centre of Mathematics and Computer Science (CWI), The Netherlands, and the National Research Institute for Computer Science and Control (INRIA), Sophia Antipolis, France.  He is currently a Lecturer with the Department of Electronic and Electrical Engineering, The University of Sheffield, U.K. His research interests include visual content analysis, visual content security, machine learning and multidimensional signal processing. He has published over 90 peer reviewed papers in leading journals, conferences and book editions. Currently, he serves as an associate editor for IEEE Transactions on Image Processing, IEEE Access and Elsevier Journal of Information Security and Applications (JISA). 

<img src="Images/charith_2022.jpg" width="150" height="200">


