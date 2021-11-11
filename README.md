# Adversarial-Learning-base-Profiled-SCA

This repository contains data and examples for reproducing the results presented in "AL-PA: Cross-Device Profiled Side-Channel Attack using
Adversarial Learning". 

In this paper, we propose a novel adversarial learning-based profiled attack (AL-PA), which enables our neural network to learn device-invariant features.
AL-PA does not require target-specific preprocessing, labeled attack traces, multiple profiling devices, and any discrepancy information of devices.

## Dataset
This cross-device dataset corresponds to an unprotected software AES-128 implementation. 

Side-channel traces are acquired from eight XMEGA chips. 
<div align="center">
	<img src="https://github.com/ALPA-SCA/Adversarial-Learning-base-Profiled-SCA/raw/main/figures/XMEGAs.jpg" alt="Editor" width="300">
  <img src="https://github.com/ALPA-SCA/Adversarial-Learning-base-Profiled-SCA/raw/main/figures/setups.jpg" alt="Editor" width="300">
</div>

The secret keys (first byte) for the eight devices are set to 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08.

## Repository structure
This repository is composed of the following folders and script:

- **./Data:** the dataset (.npy format) used in the experiments. 
- **./models**: contains the pre-trained model, final model, etc.
- **./ALPA_Demo.ipynb**: the notebook file that contains both codes and outputs. This notebook demonstrates how to load a dataset, how to pre-process the data, how to perform adversarial training, and how to evaluate the models, etc.

Note: If you cannot open the 'ALPA\_Demo.ipynb' notebook in Github, please try to open it using the nbviewer online: [https://nbviewer.org/github/ALPA-SCA/Adversarial-Learning-base-Profiled-SCA/blob/main/ALPA_Demo.ipynb](https://nbviewer.org/github/ALPA-SCA/Adversarial-Learning-base-Profiled-SCA/blob/main/ALPA_Demo.ipynb)
