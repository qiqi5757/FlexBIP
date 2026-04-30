

[📘Documentation](https://xxx/) |
[🚀Installation](https://github.com/qiqi5757/FlexBIP?tab=readme-ov-file#-get-started) |
[👀Visualization](https://github.com/qiqi5757/FlexBIP?tab=readme-ov-file#-showcase) |
[🛠️Example](https://github.com/qiqi5757/FlexBIP#%EF%B8%8F%EF%B8%8F%EF%B8%8Fexample) |
[🌟Guide](https://github.com/qiqi5757/FlexBIP#-quick-start-guide) |

 <p align="center" width="100%">
  <img src='figures/FlexBIP.png' width="100%">
</p>

## 📑 Datasets


| Dataset       | Source data                              | Data Code                                 |
|---------------|------------------------------------------|-------------------------------------------|
| PPI01         | https://doi.org/10.5281/zenodo.7600622.  | https://github.com/zqgao22/HIGH-PPI       |
| PPI02         | https://doi.org/10.5281/zenodo.13752181  | https://github.com/rui-yan/DNE            |
| PPI03         | https://tinyurl.com/networks-HuRI-paper  | https://github.com/kexinhuang12345/SkipGNN|
| DDI01         | https://go.drugbank.com/                 | https://github.com/F-windyy/DGATDDI       |
| DDI02         | https://doi.org/10.5281/zenodo.10016715  | https://github.com/LARS-research/EmerGNN  |
| DDI03         | http://snap.stanford.edu/biodata/        | https://github.com/kexinhuang12345/SkipGNN|
| DTI01         | https://zenodo.org/records/14847966      | https://github.com/CSUBioGroup/DTIAM      |
| DTI02         | https://zenodo.org/records/14847966      | https://github.com/CSUBioGroup/DTIAM      |
| DTI03         | http://snap.stanford.edu/biodata/        | https://github.com/kexinhuang12345/SkipGNN|
| DTA01         | https://zenodo.org/records/14847966      | https://github.com/CSUBioGroup/DTIAM      |
| DTA02         | https://zenodo.org/records/14847966      | https://github.com/CSUBioGroup/DTIAM      |
| circRNA-drug  | https://hanlab.tamhsc.edu/cRic/          | https://github.com/yinboliu-git/MHGTCDA   |
| drug-gene     | https://github.com/wentao228/DGCL        | https://github.com/wentao228/DGCL         |
| gene-disease  | http://www.disgenet.org/                 | https://github.com/kexinhuang12345/SkipGNN|
| miRNA-disease | http://www.cuilab.cn/hmdd                | https://github.com/a1622108/MDA-CF        |

### Dataset topological features

| Dataset | # Source Nodes | # Target Nodes | # Total Edges | # Connected Edges | Connected Edge Ratio | Max Degree |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| PPI01 | 1,553 | 1,553 | 2,411,809 | 26,640 | 0.01105 | 364 |
| PPI02 | 2,674 | 2,674 | 7,150,276 | 14,150 | 0.00198 | 140 |
| PPI03 | 5,604 | 5,604 | 31,404,816 | 46,644 | 0.00149 | 534 |
| DDI01 | 1,700 | 1,670 | 2,839,000 | 1,008,936 | 0.35538 | 1,185 |
| DDI02 | 604 | 604 | 364,816 | 57,778 | 0.15838 | 364 |
| DDI03 | 1,514 | 1,514 | 2,292,196 | 97,028 | 0.04233 | 443 |
| DTI01 | 1,384 | 5,763 | 7,975,992 | 99,884 | 0.01252 | 580 |
| DTI02 | 791 | 989 | 782,299 | 10,254 | 0.01311 | 132 |
| DTI03 | 5,018 | 2,325 | 11,666,850 | 30,280 | 0.00259 | 584 |
| DTA01 | 1,184 | 624 | 738,816 | / | / | / |
| DTA02 | 68 | 442 | 30,056 | / | / | / |
| circRNA-drug | 271 | 218 | 59,078 | 8,268 | 0.13995 | 101 |
| drug-gene | 425 | 11,006 | 4,677,550 | 65,298 | 0.01396 | 2,546 |
| miRNA-disease | 917 | 792 | 726,264 | 29,100 | 0.04007 | 384 |
| gene-disease | 9,413 | 10,370 | 97,612,810 | 163,492 | 0.00168 | 2,037 |

### Experimental Results
<p align="center">
   <img src='figures/result.tif' width="100%">
</p>



## 🚀🚀🚀Get Started

This guide will help you quickly configure and run the FlexBIP project.

#### 📦 Environment Setup


**1. Create Conda Environment:**

In the project's root directory, the `environment.yml` file defines all the necessary dependencies. Please use the following command to create the environment:


```python
conda env create -f environment.yml
```



**2. Activate the Environment:**


```
conda activate FlexBIP_env
```

**3. Install the Project Package:**

After activating the environment, run the following command to install the project itself. This will ensure all internal modules and dependencies are correctly linked.

```bash
pip install .
```

##  🛠️🛠️🛠️Example 


The training module is located at `example/main.py`. You can start the training process by running `main.py`. The training module is located at `example/main.py`. You can start the training process by running `main.py`. The dataset is located in the`example/dataset` directory. 
```python
python main.py
```
-----
##  🌟🌟🌟 Quick Start Guide
The FlexBIP model automatically adapts to the type of graph data you input. For a **homogeneous network**, you can simply set the `mode` parameter to `'I'`, while for a **heterogeneous network**, you'll set it to `'H'`.

Furthermore, you can specify the directionality of the edges using the `undirected` parameter: `undirected=True` indicates **undirected edges** (or bidirectional edges), whereas `undirected=False` indicates **directed edges** (or unidirectional edges).

Notably, the model also features **multi-task** adaptability, **automatically** determining whether to perform **binary qualitative** or **multi-class qualitative** prediction based on the data, without requiring manual configuration. This design greatly simplifies the user experience, allowing you to focus on the task itself rather than on complex model settings.

-----
## 🏆🏆🏆 Showcase
<p align="center">
   <img src='figures/visualizing surface.tif' width="100%">
<br><br>
<b>Figure 1: </b>a, Presents the surface interaction model of the protein (Q9Y6M4) and the drug (CHEMBL408982). b, The right side zooms in on the core interaction region, presenting the spatial interaction pattern between the drug molecule CHEMBL408982 (methyl carbon) and the protein residue (ASP-300, corresponding to site 300 of the Q9Y6M4 protein). 
</p>



