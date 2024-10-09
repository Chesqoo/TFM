# 🚀 Master's Thesis Experimentation Framework

## 👋 Overview

This repository contains the code used in my **Master's Thesis** on **data poisoning attacks** for models like **Phi3**, **CodeT5**, and **CodeGen**.

Feel free to use, modify, or expand upon it — just **please tag or cite my work** once my thesis is published! 😊

I’d love to know if this code helped you, whether it was to expand my research, prove something wrong, or for any other reason. 🎯

---

## 🗂 Folder Structure

Here’s an overview of the folder structure used for my experiments:

- **`datasets/`**: Contains all datasets (raw, filtered, and poisoned), divided into training, test, and validation sets.
  
- **`DNT/` (Do Not Touch)**: Stores logs and results from the experiments carried out during the thesis. It contains critical data that should not be modified, such as detailed experiment output logs.

- **`experiment_results/`**: Includes files for output samples, success rates, and the parameters used in each experiment. This folder serves as a comprehensive record of the experimental conditions and outcomes.

- **`results/`**: Contains files related to GPU VRAM usage, power consumption, and the computational cost of running the experiments. Useful for understanding resource usage during the naturalization and poisoning processes.

---

## 🛠️ Execution Order

To replicate my experiments, **run the code in the following order**:

1. **`01_DATASET_CLEANING.ipynb`**  
   Cleans and downloads the dataset.

2. **`02_DATASET_NATURALIZATION_nonNLP.ipynb`**  
   Performs naturalization (poisons the dataset and sets industry percentages).

3. **`MONITOREO.ipynb`**  
   Tracks GPU VRAM usage and power consumption and gives you an estimated cost based on the electricity price of your choosing.

After that, feel free to run any of the experiments provided for **Phi3**, **CodeT5**, and **CodeGen**.

> **Note**: These experiments are quite barebones and can definitely be improved! 🔧

---

![image](https://github.com/user-attachments/assets/8093bb04-418a-438b-9186-6b5418081b8f)  

---

## ⚡ Naturalization Details

- **`02_DATASET_NATURALIZATION.ipynb`** uses **LLaMA3** for naturalization:
  - It takes around **22 days** on an RTX 4090 to naturalize 251k rows.
  - The standard method used in **`02_DATASET_NATURALIZATION_nonNLP.ipynb`** takes around **15 seconds** to execute on the same hardware.

---

## 🔗 Thesis Link

Once my thesis is published, I’ll link it here. Stay tuned! 📖

---

## 🙌 Citation

If you use this code in your research or projects, please **cite my work** or tag me — I'd love to see how it helped! 🌟
