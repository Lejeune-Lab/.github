# Welcome to the Lejeune Lab!
This page is always under construction. :)

If you are interested in our work, you may also be interested in these links:
* [Open Access Mechanics Datasets curated from the broader mechanics community](https://elejeune11.github.io/) - please get in touch if you have datasets that you think we should add!
* [iMechanica Journal Club for May 2022: Machine Learning in Mechanics: curating datasets and defining challenge problems](https://imechanica.org/node/25935)
* [BU Mechanical Engineering PhD program](https://www.bu.edu/eng/academics/explore-degree-programs/phd-in-meche/)
* [Introduction to Computational Research at BU](https://github.com/Lejeune-Lab/BU_computational_research_intro)

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
* [List of publications with links to GitHub repositories](#pubs)
* [Resources for current and future students](#resources)

## Software projects <a name="software"></a>

| **SarcGraph** <a name="sg"></a> |
|---|
| **Description:** SarcGraph is a specialized software tool designed to streamline the detection, tracking, and analysis of z-discs and sarcomeres in movies of beating human induced pluripotent stem cell-derived cardiomyocytes (hiPSC-CMs). The main objective is to offer researchers a user-friendly, adaptable, and efficient solution for studying sarcomere dynamics in hiPSC-CMs. |
| **Paper(s):** [In Progress!]() $\bullet$ [Paper-Original](https://doi.org/10.1371/journal.pcbi.1009443) |
| **Code:** [GitHub-Latest](https://github.com/Lejeune-Lab/sarcgraph) $\bullet$ [GitHub-Legacy](https://github.com/Lejeune-Lab/Sarc-Graph) |

<p align = "center">
<img alt="datasets" src="profile/figs/SarcGraph_Example.gif" width="50%" />
</p>

| **MicroBundleCompute** <a name="mbc"></a> |
|---|
| **Description:** This software is developed as a multi-purpose tool for analyzing heterogeneous cardiac microbundle deformation and strain from brightfield movies of beating microbundles. Specifically, the software is able to automatically generate a mask of the microbundle component of the movie frames, identify tracking points as Shi-Tomasi corner points in this region of interest, and track the fiducial points across all frames. From the tracked positions of the fiducial points, we are able to compute full-field displacements, subdomain-averaged strains, and strain-derived results. We also include post-processing functionalities to rotate the images and tracking results as well as interpolate the output at query points. To visualize the output, the software generates timeseries plots per beat and movies of full-field and subdomain-averaged results.|
| **Paper(s):** in preparation |
| **Code:** https://github.com/HibaKob/MicroBundleCompute |

<p align = "center">
<img alt="datasets" src="profile/figs/MicroBundleCompute_Example.gif" width="50%" />
</p>

| **WoundCompute** <a name="wc"></a> |
|---|
| **Description:** This software is designed to analyze experimental data from micro-tissue wound experiments. The goal of our software is to extract quantitative information from these images and movies. For example, we can automatically identify the wound region which allows us extract properties such as wound area, major axis length, and minor axis length with respect to time. We can also automatically identify tissue properties such as tissue width, and tissue edge curvature, determine if the tissue is broken (i.e., detached from posts) or if the wound is closed. |
| **Paper(s):** in preparation. |
| **Code:** https://github.com/elejeune11/woundcompute |

<p align = "center">
<img alt="datasets" src="profile/figs/software_example.gif" width="50%" />
</p>

| **FEniCS ArcLength** <a name="fenics"></a> |
|---|
| **Description:** fenics-arclength is a Python implementation of the arclength solver built on top of FEniCS. The Arc Length Method, sometimes referred to as the Riks Method, is a method used to solve solid mechanics problems with geometric nonlinearity with complex equilibrium paths. The library aims to keep the usage as similiar to FEniCS (version 2019.1.0) to allow for off-the-shelf implementation and integration with other FEniCS workflows. |
| **Paper(s):** In progress |
| **Code:** https://github.com/pprachas/fenics_arclength |

| **Autotwin** <a name="autotwin"></a> |
|---|
| **Description:** The goal of this project is to create a fully automated workflow from head MRI $\mapsto$ segmented isosurfaces $\mapsto$ FEA mesh $\mapsto$ FEA simulation for the purpose of understanding subject specific traumatic brain injury risk. |
| **Paper(s):** n/a |
| **Code:** https://github.com/autotwin |

## Datasets <a name="data"></a>

In our group, we have created and disseminated multiple open access mechanics datasets for assessing the performance of machine learning models. All datasets are created with open source finite element software [FEniCS](https://fenicsproject.org/), and all are shared under [CC BY SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) licenses. Please feel free to download and use them for any research or educational purposes!

<p align = "center">
<img alt="datasets" src="profile/figs/datasets.png" width="75%" />
</p>

| **Mechanical MNIST - Uniaxial Extension, Shear, Confined Compression, Equibiaxial Extension** <a name="m-mnist"></a>|
|---|
| **Description:** Each dataset in the Mechanical MNIST collection contains the results of 70,000 (60,000 training examples + 10,000 test examples) finite element simulation of a heterogeneous material subject to large deformation. Mechanical MNIST is generated by first converting the [MNIST bitmap images](http://www.pymvpa.org/datadb/mnist.html) to 2D heterogeneous blocks of material. There are four different load cases provided. |
| **Link(s):** [Uniaxial Extension](https://open.bu.edu/handle/2144/38693) $\bullet$ [Shear](https://open.bu.edu/handle/2144/39429) $\bullet$ [Confined Compression](https://open.bu.edu/handle/2144/39427) $\bullet$ [Equibiaxial Extension](https://open.bu.edu/handle/2144/39428) |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.eml.2020.100659) $\bullet$ [Open Access](https://open.bu.edu/handle/2144/39813) |
| **Code:** [GitHub](https://github.com/Lejeune-Lab/Mechanical-MNIST) |

| **Mechanical MNIST - Multi-Fidelity** |
|---|
| **Description:** This dataset builds directly on the format of the original Mechanical MNIST dataset. Here, we provide data from FEA simulations with unrefined meshes for the purpose of testing the efficacy of multi-fidelity modeling (i.e., transfer learning) approaches. |
| **Link(s):** https://open.bu.edu/handle/2144/41357 |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.jmbbm.2020.104276) $\bullet$ [Open Access](https://open.bu.edu/handle/2144/43423) |
| **Code:** [GitHub](https://github.com/Lejeune-Lab/Mechanical-MNIST-Transfer-Learning) |

| **Mechanical MNIST - Fashion** |
|---|
| **Description:** Each dataset in the Mechanical MNIST collection contains the results of 70,000 (60,000 training examples + 10,000 test examples) finite element simulation of a heterogeneous material subject to large deformation. Mechanical MNIST - Fashion is generated by first converting the [fashion MNIST bitmap images](https://github.com/zalandoresearch/fashion-mnist) to 2D heterogeneous blocks of material. |
| **Link(s):** https://open.bu.edu/handle/2144/41450 |
| **Original paper:** n/a, first used [here](https://arxiv.org/abs/2108.03995) |
| **Code:** [GitHub](https://github.com/Lejeune-Lab/Mechanical-MNIST-fashion) |

| **Mechanical MNIST - Crack Path** |
|---|
| **Description:** The Mechanical MNIST Crack Path dataset contains Finite Element simulation results from phase-field models of quasi-static brittle fracture in heterogeneous material domains subjected to prescribed loading and boundary conditions. |
| **Link(s):** https://open.bu.edu/handle/2144/42757 |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.eml.2021.101566) $\bullet$ [Open Access](https://arxiv.org/abs/2108.03995) |
| **Code:** [GitHub-Dataset](https://github.com/Lejeune-Lab/Mechanical-MNIST-Crack-Path) $\bullet$ [GitHub-Metamodel](https://github.com/Lejeune-Lab/MultiRes-WNet) |

| **Mechanical MNIST - Cahn-Hilliard** |
|---|
| **Description:** The Mechanical MNIST Cahn-Hilliard dataset contains the results of 104,813 Finite Element simulations of a heterogeneous material domain subject to large equibiaxial extension deformation. The heterogeneous domain patterns are generated from a Finite Element implementation of the Cahn-Hilliard equation. Both stripe and circle patterns are present in the dataset. |
| **Link(s):** https://open.bu.edu/handle/2144/43971 |
| **Original paper:** [Journal Link](https://doi.org/10.1115/1.4054898) $\bullet$ [Open Access](https://arxiv.org/abs/2203.04183) |
| **Code:** https://github.com/Lejeune-Lab/Mechanical-MNIST-Cahn-Hilliard |

| **Mechanical MNIST - Distribution Shift** |
|---|
| **Description:** The Mechanical MNIST – Distribution Shift dataset is specifically designed to demonstrate three types of data distribution shift: (1) covariate shift, (2) mechanism shift, and (3) sampling bias, for all of which the training and testing environments are drawn from different distributions. For each type of data distribution shift, we have one dataset generated from the Mechanical MNIST bitmaps and one from the Mechanical MNIST – EMNIST Letters bitmaps. |
| **Link(s):** https://open.bu.edu/handle/2144/44485 |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.cma.2022.115569) $\bullet$ [Open Access](https://arxiv.org/abs/2206.14917) |
| **Code:** https://github.com/Lejeune-Lab/ood_mechanics |

| **Buckling Instability Classification (BIC)** <a name="bic"></a> |
|---|
| **Description:** The Buckling Instability Classification (BIC) datasets contain the results of finite element simulations where a heterogeneous column is subject to a fixed level of applied displacement and is classified as either "Stable" or "Unstable." Each model input is a 16x1 vector where the entries of the vector dictate the Young's Modulus (E) of the corresponding portion of the physical column domain. There are three sub-datasets with different input property distributions: BIC-1, BIC-2, and BIC-3. |
| **Link(s):** https://open.bu.edu/handle/2144/40085 |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.cad.2020.102948) $\bullet$ [Open Access](https://sites.bu.edu/lejeunelab/files/2021/02/BIC.pdf)|
| **Code:** [GitHub](https://github.com/Lejeune-Lab/BIC) |

| **Asymmetric Buckling Columns (ABC)** <a name="abc"></a>|
|---|
| **Description:** The Asymmetric Buckling Columns (ABC) dataset contains spatially heterogeneous columns with fixed-fixed boundary conditions that are classified to be buckling left (label of 0) or right (label of 1). The dataset is split into 3 subdatasets: sub-dataset 1, sub-dataset 2, and sub-dataset 3, each with increasing levels of geometric complexity. |
| **Link(s):** https://open.bu.edu/handle/2144/43730 |
| **Original paper:** [Journal Link](https://doi.org/10.1016/j.compstruc.2022.106825) $\bullet$ [Open Access](https://arxiv.org/abs/2202.01380) |
| **Code:** https://github.com/Lejeune-Lab/ABC_dataset |

## Publications + relevant GitHub repositories <a name="pubs"></a>

TODO: figure out what to link to here -- e.g., link to manuscript, link to repo for ML models in paper -- forked? -- link to datasets/software? or do we just reference above? 

* Yuan, L., Park, H. S., & Lejeune, E. (2022). Towards out of distribution generalization for problems in mechanics. Computer Methods in Applied Mechanics and Engineering, 400, 115569.\[[paper](https://doi.org/10.1016/j.cma.2022.115569)\]\[[code](https://github.com/Lejeune-Lab/ood_mechanics)\]\|\[[data](https://open.bu.edu/handle/2144/44485)\]
* Das, S. L., Sutherland, B. P., Lejeune, E., Eyckmans, J., & Chen, C. S. (2022). Mechanical response of cardiac microtissues to acute localized injury. American Journal of Physiology-Heart and Circulatory Physiology.
* Prachaseree, P., & Lejeune, E. (2022). Learning Mechanically Driven Emergent Behavior with Message Passing Neural Networks. Computers & Structures, 270, 106825. 
* Kobeissi, H., Mohammadzadeh, S., & Lejeune, E. (2022). Enhancing Mechanical Metamodels with a Generative Model-Based Augmented Training Dataset. Journal of Biomechanical Engineering.
* Mohammadzadeh, S., & Lejeune, E. (2021). Predicting mechanically driven full-field Quantities of Interest with deep learning-based metamodels. Extreme Mechanics Letters, 101566. [[paper](https://www.sciencedirect.com/science/article/pii/S2352431621002303) $\bullet$ [Data-Light](https://open.bu.edu/handle/2144/42757) $\bullet$ [Data-Extended](https://datadryad.org/stash/dataset/doi:10.5061/dryad.rv15dv486)]
* Zhao B., Zhang K., Chen C.S., & Lejeune E. (2021) Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Comput Biol 17(10): e1009443. 
* Lejeune, E., & Zhao, B. (2021). Exploring the potential of transfer learning for metamodels of heterogeneous material deformation. Journal of the Mechanical Behavior of Biomedical Materials, 104276.
* Lejeune, E. (2021). Geometric stability classification: datasets, metamodels, and adversarial attacks. Computer-Aided Design, 131, 102948.
* Kakaletsis, S., Meador, W. D., Mathur, M., Sugerman, G. P., Jazwiec, T., Malinowski, M., Lejeune, E., Timek, T.A., & Rausch, M. K. (2020). Right Ventricular Myocardial Mechanics: Multi-Modal Deformation, Microstructure, Modeling, and Comparison to the Left Ventricle. Acta Biomaterialia.
* Lejeune, E. (2020). Mechanical MNIST: A benchmark dataset for mechanical metamodels. Extreme Mechanics Letters, 100659. 


## Resources for current and future students <a name="resources"></a>

[Introduction to Lejeune Lab computational research, including recommended courses and how to get started with using the SCC](https://github.com/Lejeune-Lab/BU_computational_research_intro)

[Lessons on bringing your computational research skills to the next level from our collaborator Chad Hovey at SNL](https://github.com/autotwin/lessons)

[A simple tutorial on curve fitting in the context of constitutive modeling with Python](https://github.com/elejeune11/fitting-one-term-ogden-model)

[Notes on non-linear FEA with FEniCS](https://fenics-arclength.readthedocs.io/en/latest/math_prelim.html) and [Notes on geometrically exact beams (Simo-Reissner) with FEniCS](https://fenics-arclength.readthedocs.io/en/latest/examples/force_control/beam/README.html#)
