# FINER
This repository contains the code and data associated with the CCS'23 publication. An extended version of the paper, including an appendix, can be found on [arXiv](https://arxiv.org/pdf/2308.05362.pdf).

<img src=functionLocation.png width=90% />

A sample output from our tool, which is valuable for malware analysis in achieving

&#x2705; High Fidelity: locate malicious functionalities  correctly with high confidence;

&#x2705; High Intelligibility: generate explanations at a high abstraction level, e.g., functions instead of opcode features.

## Setup

```shell
conda env create --name FINER --file finer.yml
conda activate FINER
```

## How to run

All scripts can be found in `test/`. To run the experiments, use 

```shell
python -m unittest test/test_damd.py
python -m unittest test/test_deepreflect.py
python -m unittest test/test_vuldeepecker.py
```

## Citation

If you find this research helpful for your publications, please kindly cite: 
```
@inproceedings{he2023finer,
  title={FINER: Enhancing State-of-the-art Classifiers with Feature Attribution to Facilitate Security Analysis},
  author={He, Yiling and Lou, Jian and Qin, Zhan and Ren, Kui},
  booktitle={Proceedings of the 2023 ACM SIGSAC Conference on Computer and Communications Security},
  pages={416--430},
  year={2023}
}
```
