# Welcome to the Lejeune Lab!
This page is under construction. :)

If you are interested in our work, you may also be interested in these links:
* Open Access Mechanics Datasets https://elejeune11.github.io/
* iMechanica Journal Club for May 2022: Machine Learning in Mechanics: curating datasets and defining challenge problems https://imechanica.org/node/25935
* BU Mechanical Engineering PhD program: https://www.bu.edu/eng/academics/explore-degree-programs/phd-in-meche/


## Table of contents
* [Software projects](#software)
    * [SarcGraph sarcomere tracking in hiPSC-CMs](#sg)
    * [MicroBundleCompute cardiac microtissue mechanical metrics](#mbc)
    * [WoundCompute three-dimensional wound healing analysis software](#wc)
    * [FEniCS ArcLength solver](#fenics)
    * [Autotwin MRI to mesh to TBI simulation](#autotwin)
* [Datasets](#data)
    * [Mechanical MNIST Collection](#m-mnist)
    * [Buckling Instability Classification (BIC)](#bic)
    * [Asymmetric Buckling Columns (ABC)](#abc)
* [List of publications with links to the relevant GitHub repository](#pubs)
* [Resources for current and future students (public)](#resources)

## Software projects <a name="software"></a>

### SarcGraph <a name="sg"></a>
[old sarcgraph](https://github.com/Lejeune-Lab/Sarc-Graph)

### MicroBundleCompute <a name="mbc"></a>

### WoundCompute <a name="wc"></a>

### FEniCS ArcLength <a name="fenics"></a>

### Autotwin <a name="autotwin"></a>

## Datasets <a name="data"></a>

In our group, we have created and disseminated multiple open access mechanics datasets for assessing the performance of machine learning models. All datasets are created with open source finite element software [FEniCS](https://fenicsproject.org/), and all are shared under [CC BY SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) licenses. Please feel free to download and use them for any research or educational purposes!

<p align = "center">
<img alt="datasets" src="profile/figs/datasets.png" width="75%" />
</p>

### Mechanical MNIST Collection <a name="m-mnist"></a>

Will create one small table for each individual dataset within the collection.

### Buckling Instability Classification (BIC) <a name="bic"></a>

| **Buckling Instability Classification (BIC)** |
|---|
| **Description:** The Buckling Instability Classification (BIC) datasets contain the results of finite element simulations where a heterogeneous column is subject to a fixed level of applied displacement and is classified as either "Stable" or "Unstable." Each model input is a 16x1 vector where the entries of the vector dictate the Young's Modulus (E) of the corresponding portion of the physical column domain. There are three sub-datasets with different input property distributions: BIC-1, BIC-2, and BIC-3. |
| **Link(s):** https://open.bu.edu/handle/2144/40085 |
| **Original paper:** https://doi.org/10.1016/j.cad.2020.102948 |
| **Code:** do we fork repo first? |

### Asymmetric Buckling Columns (ABC) <a name="abc"></a>

| **Asymmetric Buckling Columns (ABC)** |
|---|
| **Description:** To fill in. |
| **Link(s):** To fill in. |
| **Original paper:** To fill in. |
| **Code:** To fill in. |

## Publications + relevant GitHub repositories <a name="pubs"></a>

TODO: figure out what to link to here -- e.g., link to manuscript, link to repo for ML models in paper -- forked? -- link to datasets/software? or do we just reference above? 

* Yuan, L., Park, H. S., & Lejeune, E. (2022). Towards out of distribution generalization for problems in mechanics. Computer Methods in Applied Mechanics and Engineering, 400, 115569.
* Das, S. L., Sutherland, B. P., Lejeune, E., Eyckmans, J., & Chen, C. S. (2022). Mechanical response of cardiac microtissues to acute localized injury. American Journal of Physiology-Heart and Circulatory Physiology.
* Prachaseree, P., & Lejeune, E. (2022). Learning Mechanically Driven Emergent Behavior with Message Passing Neural Networks. Computers & Structures, 270, 106825. 
* Kobeissi, H., Mohammadzadeh, S., & Lejeune, E. (2022). Enhancing Mechanical Metamodels with a Generative Model-Based Augmented Training Dataset. Journal of Biomechanical Engineering.
* Mohammadzadeh, S., & Lejeune, E. (2021). Predicting mechanically driven full-field Quantities of Interest with deep learning-based metamodels. Extreme Mechanics Letters, 101566.
* Zhao B., Zhang K., Chen C.S., & Lejeune E. (2021) Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Comput Biol 17(10): e1009443. 
* Lejeune, E., & Zhao, B. (2021). Exploring the potential of transfer learning for metamodels of heterogeneous material deformation. Journal of the Mechanical Behavior of Biomedical Materials, 104276.
* Lejeune, E. (2021). Geometric stability classification: datasets, metamodels, and adversarial attacks. Computer-Aided Design, 131, 102948.
* Kakaletsis, S., Meador, W. D., Mathur, M., Sugerman, G. P., Jazwiec, T., Malinowski, M., Lejeune, E., Timek, T.A., & Rausch, M. K. (2020). Right Ventricular Myocardial Mechanics: Multi-Modal Deformation, Microstructure, Modeling, and Comparison to the Left Ventricle. Acta Biomaterialia.
* Lejeune, E. (2020). Mechanical MNIST: A benchmark dataset for mechanical metamodels. Extreme Mechanics Letters, 100659. 


## Resources for current and future students <a name="resources"></a>

Introduction to Lejeune Lab computational research, including recommended courses and how to get started with using the SCC:
https://github.com/Lejeune-Lab/BU_computational_research_intro 

Lessons on bringing your computational research skills to the next level from our collaborator Chad Hovey at SNL: https://github.com/autotwin/lessons

A simple tutorial on curve fitting in the context of constitutive modeling with Python: https://github.com/elejeune11/fitting-one-term-ogden-model

Notes on non-linear FEA and geometrically exact beams (Simo-Reissner) in the context of FEniCS: https://fenics-arclength.readthedocs.io/en/latest/math_prelim.html and https://fenics-arclength.readthedocs.io/en/latest/examples/force_control/beam/README.html#


