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
