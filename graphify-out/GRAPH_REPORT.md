# Graph Report - papers  (2026-04-29)

## Corpus Check
- Corpus is ~0 words - fits in a single context window. You may not need a graph.

## Summary
- 322 nodes · 393 edges · 24 communities detected
- Extraction: 96% EXTRACTED · 3% INFERRED · 1% AMBIGUOUS · INFERRED: 11 edges (avg confidence: 0.82)
- Token cost: 36,700 input · 8,300 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Bayesian Seismic Inversion|Bayesian Seismic Inversion]]
- [[_COMMUNITY_FWI & Deep Learning|FWI & Deep Learning]]
- [[_COMMUNITY_Velocity Model Building|Velocity Model Building]]
- [[_COMMUNITY_Seismic Fault Interpretation|Seismic Fault Interpretation]]
- [[_COMMUNITY_3D FWI Neural Architecture|3D FWI Neural Architecture]]
- [[_COMMUNITY_Residual Statics HRNet|Residual Statics HRNet]]
- [[_COMMUNITY_Ediacaran Geochemistry|Ediacaran Geochemistry]]
- [[_COMMUNITY_GAN Seismic Noise Attenuation|GAN Seismic Noise Attenuation]]
- [[_COMMUNITY_CMP Gather Processing|CMP Gather Processing]]
- [[_COMMUNITY_InversionNet3D Team|InversionNet3D Team]]
- [[_COMMUNITY_Low-Data Learning Strategies|Low-Data Learning Strategies]]
- [[_COMMUNITY_Geological Constraints MTL|Geological Constraints MTL]]
- [[_COMMUNITY_XAI & Interpretability|XAI & Interpretability]]
- [[_COMMUNITY_Normalizing Flows|Normalizing Flows]]
- [[_COMMUNITY_Reversible Networks|Reversible Networks]]
- [[_COMMUNITY_GAN Architectures|GAN Architectures]]
- [[_COMMUNITY_VGG Backbone|VGG Backbone]]
- [[_COMMUNITY_Supervised Learning|Supervised Learning]]
- [[_COMMUNITY_Image Classification|Image Classification]]
- [[_COMMUNITY_Data Quality Challenges|Data Quality Challenges]]
- [[_COMMUNITY_2D vs 3D CNN|2D vs 3D CNN]]
- [[_COMMUNITY_Single-Target Networks|Single-Target Networks]]
- [[_COMMUNITY_IEEE TGRS Journal|IEEE TGRS Journal]]
- [[_COMMUNITY_Geophysics Journal|Geophysics Journal]]

## God Nodes (most connected - your core abstractions)
1. `Hosseinzadeh et al. 2025 - Seismic inversion approaches for reservoir characterization (J. Applied Geophysics)` - 43 edges
2. `Dong et al. 2024 - Ediacaran palaeo-ocean environment (Earth-Science Reviews)` - 24 edges
3. `Physics-Guided Data-Driven Seismic Inversion: Recent Progress and Future Opportunities in Full-Waveform Inversion (Lin et al., 2023)` - 23 edges
4. `Full Waveform Inversion (FWI)` - 13 edges
5. `Physics-Guided Deep Autoencoder to Overcome the Need for a Starting Model in Full-Waveform Inversion (Dhara & Sen, 2022)` - 11 edges
6. `Orozco et al. 2024 - Machine Learning Enabled Velocity Model Building with Uncertainty Quantification` - 10 edges
7. `An Empirical Study of Large-Scale Data-Driven Full Waveform Inversion (Jin et al., 2024)` - 9 edges
8. `Kaur, Fomel & Pham 2020/2021 - Seismic Ground-Roll Noise Attenuation Using Deep Learning` - 9 edges
9. `OpenFWI: Large-scale Multi-structural Benchmark Datasets for Full Waveform Inversion (Deng et al., 2022)` - 8 edges
10. `Physics-Informed Neural Networks (PINNs) for Wave Propagation and Full Waveform Inversions (Rasht-Behesht et al., 2022)` - 8 edges

## Surprising Connections (you probably didn't know these)
- `Salt Body Velocity Inversion` --semantically_similar_to--> `ASPIRE Algorithm (Iterative Amortized Posterior Inference for Bayesian Inverse Problems)`  [INFERRED] [semantically similar]
  papers/cluster_B_VelocityModelBuilding/B3_AlAli & Anifowose_2022.pdf → papers/cluster_B_VelocityModelBuilding/B5_Orozco et al._2024.pdf
- `Synergizing Deep Learning and Full-Waveform Inversion: Bridging Data-Driven and Theory-Guided Approaches for Enhanced Seismic Imaging (Zerafa et al., 2025)` --discusses--> `3D Full Waveform Inversion`  [INFERRED]
  papers/cluster_A_FWI_DeepLearning/A6_Zerafa et al._2025.pdf → papers/cluster_A_FWI_DeepLearning/A2_Lin et al._2023.pdf
- `Physics-Informed Neural Networks (PINNs)` --semantically_similar_to--> `Physics-Guided Deep Autoencoder for FWI (Dhara & Sen approach)`  [INFERRED] [semantically similar]
  papers/cluster_A_FWI_DeepLearning/A3_Rasht-Behesht et al._2022.pdf → papers/cluster_A_FWI_DeepLearning/A5_Dhara & Sen_2022.pdf
- `UPFWI: Unsupervised Physics-informed Full Waveform Inversion` --semantically_similar_to--> `Physics-Guided Deep Autoencoder for FWI (Dhara & Sen approach)`  [INFERRED] [semantically similar]
  papers/cluster_A_FWI_DeepLearning/A2_Lin et al._2023.pdf → papers/cluster_A_FWI_DeepLearning/A5_Dhara & Sen_2022.pdf
- `AlAli & Anifowose 2022 - Seismic Velocity Modeling in the Digital Transformation Era: A Review of ML` --semantically_similar_to--> `Orozco et al. 2024 - Machine Learning Enabled Velocity Model Building with Uncertainty Quantification`  [INFERRED] [semantically similar]
  papers/cluster_B_VelocityModelBuilding/B3_AlAli & Anifowose_2022.pdf → papers/cluster_B_VelocityModelBuilding/B5_Orozco et al._2024.pdf

## Hyperedges (group relationships)
- **Unsupervised physics-guided FWI: three approaches sharing the pattern of (1) no labeled velocity-seismic pairs, (2) physics constraint replaces supervision, (3) CNN-based architecture** — concept_upfwi, concept_deep_autoencoder_fwi, concept_physics_informed_neural_networks [INFERRED 0.85]
- **OpenFWI benchmark ecosystem: dataset (A1), review contextualizing it (A2), and scaling study on it (A4) form a coherent research platform for data-driven FWI** — a1_deng_et_al_2022_paper, concept_openfwi_dataset, a4_jin_et_al_2024_paper, concept_bigfwi [INFERRED 0.90]
- **PGML-FWI taxonomy: Lin et al. 2023 review categorizes A3 (PINN), A5 (autoencoder FWI), and UPFWI all as physics-guided approaches under a unified six-category framework** — a2_lin_et_al_2023_paper, a3_rasht_behesht_et_al_2022_paper, a5_dhara_sen_2022_paper, concept_physics_guided_machine_learning [EXTRACTED 0.95]
- **ML-Based Velocity Model Building Pipeline: FWI + ML supervision + Physical constraints** — b3_full_waveform_inversion, b3_machine_learning_velocity, b3_low_freq_extrapolation, b5_aspire_algorithm, b5_common_image_gathers [INFERRED 0.82]
- **GAN-Based Seismic Data Processing: Ground-Roll Attenuation, Trace Interpolation, CycleGAN Architecture** — c1_kaur_et_al_2021_paper, c3_kaur_pham_fomel_2021_paper, c1_gan_seismic, c3_gan_interpolation, c1_cyclegan_architecture [INFERRED 0.88]
- **Bayesian Framework for Seismic Inversion with Uncertainty: SBI + Diffusion Networks + Physics Summary Statistics** — b5_simulation_based_inference, b5_diffusion_networks_velocity, b5_common_image_gathers, b5_bayesian_uncertainty_quantification, b5_amortized_inference [EXTRACTED 0.95]
- **D3 covers all major seismic inversion method families** —  [INFERRED 1.00]
- **Uncertainty quantification methods for seismic inversion** —  [INFERRED 0.90]
- **Geochemical proxies used to reconstruct Ediacaran paleoenvironment in D2** —  [INFERRED 1.00]
- **Machine learning approaches for seismic inversion** —  [INFERRED 1.00]

## Communities

### Community 0 - "Bayesian Seismic Inversion"
Cohesion: 0.06
Nodes (52): Bachrach 2006 - Stochastic rock physics modelling + Bayesian, Bosch et al. 2010 - Elastic seismic inversion (Llanos Basin), Connolly 1999 - Elastic impedance, Das et al. 2019 - CNN seismic inversion for P-impedance, Grana 2016 - Bayesian rock-physics inversion (analytical), Grana & Della Rossa 2010 - Bayesian petrophysical inversion, Johansen et al. 2013 - Numerical inverse rock physics, Johari & Emami Niri 2021 - Rock physics diagnostic and RPT (+44 more)

### Community 1 - "FWI & Deep Learning"
Cohesion: 0.09
Nodes (46): OpenFWI: Large-scale Multi-structural Benchmark Datasets for Full Waveform Inversion (Deng et al., 2022), Physics-Guided Data-Driven Seismic Inversion: Recent Progress and Future Opportunities in Full-Waveform Inversion (Lin et al., 2023), Physics-Informed Neural Networks (PINNs) for Wave Propagation and Full Waveform Inversions (Rasht-Behesht et al., 2022), An Empirical Study of Large-Scale Data-Driven Full Waveform Inversion (Jin et al., 2024), Physics-Guided Deep Autoencoder to Overcome the Need for a Starting Model in Full-Waveform Inversion (Dhara & Sen, 2022), Synergizing Deep Learning and Full-Waveform Inversion: Bridging Data-Driven and Theory-Guided Approaches for Enhanced Seismic Imaging (Zerafa et al., 2025), Arnab Dhara (University of Texas at Austin), George Em Karniadakis (Brown University) (+38 more)

### Community 2 - "Velocity Model Building"
Cohesion: 0.07
Nodes (37): Chen et al. 2021 - Velocity Model Building (cluster B1, file inaccessible - Microsoft login redirect), Geng et al. 2022 - Velocity Model Building (cluster B2, file misdirected to GPS deformation paper), AlAli & Anifowose 2022 - Seismic Velocity Modeling in the Digital Transformation Era: A Review of ML, BP 2004 Velocity Model (Benchmark Dataset), Convolutional Neural Network (CNN) for Velocity Estimation, Cycle-Skipping Problem in FWI, DBSCAN Clustering for Velocity Picking, Well-Log Facies-Based Regularization for FWI (+29 more)

### Community 3 - "Seismic Fault Interpretation"
Cohesion: 0.06
Nodes (37): An and Dong (2023) - Prior Knowledge in CNN Fault Interpretation, An et al. (2021) - Deep CNN for Fault Recognition, Bayesian Neural Network (BNN), Challenge C7: Imbalanced Classification, Convolutional Neural Network (CNN), Conrad Childs, Dairui Liu, Deep Learning (DL) (+29 more)

### Community 4 - "3D FWI Neural Architecture"
Cohesion: 0.06
Nodes (32): 3D Full Waveform Inversion, AdamW, Additive Coupling, Batch Normalization, Channel-Separated Encoder, Channel Shuffle, Depthwise Convolution, DOE-EDX Platform (+24 more)

### Community 5 - "Residual Statics HRNet"
Cohesion: 0.07
Nodes (27): GeoScienceWorld / Society of Exploration Geophysicists (SEG), TomoPlus (GeoTomo), Jie Zhang, National Key R&D Program of China, Reflection residual statics estimated using a high-resolution neural network, Prestack Time Migration, Residual statics solution by L1 regularized inversion in common offset domain (Duan and Zhang 2017), 3D seismic residual statics solutions derived from refraction interferometry (Gao and Zhang 2017) (+19 more)

### Community 6 - "Ediacaran Geochemistry"
Cohesion: 0.09
Nodes (24): Bingshuang Zhao, Bohao Dong, Chao Cheng, Hong Hua, Jie Li, Xiaoping Long, Yunpeng Dong, Cloudina fauna (+16 more)

### Community 7 - "GAN Seismic Noise Attenuation"
Cohesion: 0.14
Nodes (17): CycleGAN Architecture for Seismic Noise Attenuation, Generative Adversarial Networks (GANs) for Seismic Processing, Ground-Roll Noise Attenuation, Kaur, Fomel & Pham 2020/2021 - Seismic Ground-Roll Noise Attenuation Using Deep Learning, Land Seismic Data (Ground-Roll Contaminated), Local Time-Frequency (LTF) Transform, Plane-Wave Destruction (PWD) Filters, Regularized Non-Stationary Regression (RNR) (+9 more)

### Community 8 - "CMP Gather Processing"
Cohesion: 0.12
Nodes (17): Common Midpoint (CMP) Gather, Surface-Consistency-Based Data Augmentation, Deep Learning Residual Statics Estimation Method, Group Normalization, NVIDIA GTX 1080Ti GPU, HRNet (High-Resolution Neural Network), Normal Moveout (NMO) Correction, PetroChina (+9 more)

### Community 9 - "InversionNet3D Team"
Cohesion: 0.27
Nodes (10): Brendt Wohlberg, GeoDNN, InversionNet3D: Efficient and Scalable Learning for 3D Full Waveform Inversion, Los Alamos National Laboratory, NNFWI, Qili Zeng, SeisInvNet, Shihang Feng (+2 more)

### Community 10 - "Low-Data Learning Strategies"
Cohesion: 0.29
Nodes (7): Active Learning, Challenge C1: Lack of Annotated Data, Human-in-the-Loop Approach, Knowledge Distillation, Semi-Supervised Learning, Synthetic Seismic Data Generation, Transfer Learning

### Community 11 - "Geological Constraints MTL"
Cohesion: 0.67
Nodes (3): Challenge C11: Omission of Geological Constraints, Fault Probability Map, Multi-Task Learning (MTL)

### Community 12 - "XAI & Interpretability"
Cohesion: 1.0
Nodes (2): Challenge C6: Lack of Interpretability, Explainable Artificial Intelligence (XAI)

### Community 13 - "Normalizing Flows"
Cohesion: 1.0
Nodes (1): Real NVP

### Community 14 - "Reversible Networks"
Cohesion: 1.0
Nodes (1): Reversible Residual Network

### Community 15 - "GAN Architectures"
Cohesion: 1.0
Nodes (1): Generative Adversarial Network (GAN)

### Community 16 - "VGG Backbone"
Cohesion: 1.0
Nodes (1): VGG Network

### Community 17 - "Supervised Learning"
Cohesion: 1.0
Nodes (1): Supervised Learning

### Community 18 - "Image Classification"
Cohesion: 1.0
Nodes (1): Image Classification

### Community 19 - "Data Quality Challenges"
Cohesion: 1.0
Nodes (1): Challenge C2: Poor Data Quality

### Community 20 - "2D vs 3D CNN"
Cohesion: 1.0
Nodes (1): 2D vs 3D CNN for Seismic Fault Interpretation

### Community 21 - "Single-Target Networks"
Cohesion: 1.0
Nodes (1): Single Target Single Network (STSN)

### Community 22 - "IEEE TGRS Journal"
Cohesion: 1.0
Nodes (1): IEEE Transactions on Geoscience and Remote Sensing

### Community 23 - "Geophysics Journal"
Cohesion: 1.0
Nodes (1): Geophysics

## Ambiguous Edges - Review These
- `Chen et al. 2021 - Velocity Model Building (cluster B1, file inaccessible - Microsoft login redirect)` → `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B1_Chen et al._2021.pdf · relation: AMBIGUOUS_may_address
- `Geng et al. 2022 - Velocity Model Building (cluster B2, file misdirected to GPS deformation paper)` → `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B2_Geng et al._2022.pdf · relation: AMBIGUOUS_may_address
- `Alkhalifah et al. 2021 - Velocity Model Building (cluster B4, file misdirected to PV-RAFT point cloud paper)` → `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B4_Alkhalifah et al._2021.pdf · relation: AMBIGUOUS_may_address

## Knowledge Gaps
- **42 isolated node(s):** `VelocityGAN (GAN-based FWI)`, `Marmousi Velocity Model (2D seismic benchmark)`, `SEG Advanced Modeling Corporation (SEAM) Phase 1 Salt Model`, `SpecFem2D (spectral element wave simulation code)`, `Kimberlina CO2 Sequestration Dataset` (+37 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `XAI & Interpretability`** (2 nodes): `Challenge C6: Lack of Interpretability`, `Explainable Artificial Intelligence (XAI)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normalizing Flows`** (1 nodes): `Real NVP`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Reversible Networks`** (1 nodes): `Reversible Residual Network`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `GAN Architectures`** (1 nodes): `Generative Adversarial Network (GAN)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `VGG Backbone`** (1 nodes): `VGG Network`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Supervised Learning`** (1 nodes): `Supervised Learning`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Image Classification`** (1 nodes): `Image Classification`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Data Quality Challenges`** (1 nodes): `Challenge C2: Poor Data Quality`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `2D vs 3D CNN`** (1 nodes): `2D vs 3D CNN for Seismic Fault Interpretation`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Single-Target Networks`** (1 nodes): `Single Target Single Network (STSN)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `IEEE TGRS Journal`** (1 nodes): `IEEE Transactions on Geoscience and Remote Sensing`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Geophysics Journal`** (1 nodes): `Geophysics`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Chen et al. 2021 - Velocity Model Building (cluster B1, file inaccessible - Microsoft login redirect)` and `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`?**
  _Edge tagged AMBIGUOUS (relation: AMBIGUOUS_may_address) - confidence is low._
- **What is the exact relationship between `Geng et al. 2022 - Velocity Model Building (cluster B2, file misdirected to GPS deformation paper)` and `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`?**
  _Edge tagged AMBIGUOUS (relation: AMBIGUOUS_may_address) - confidence is low._
- **What is the exact relationship between `Alkhalifah et al. 2021 - Velocity Model Building (cluster B4, file misdirected to PV-RAFT point cloud paper)` and `Full-Waveform Inversion (FWI) - Shared Cross-Paper Concept`?**
  _Edge tagged AMBIGUOUS (relation: AMBIGUOUS_may_address) - confidence is low._
- **Why does `Hosseinzadeh et al. 2025 - Seismic inversion approaches for reservoir characterization (J. Applied Geophysics)` connect `Bayesian Seismic Inversion` to `Ediacaran Geochemistry`?**
  _High betweenness centrality (0.046) - this node is a cross-community bridge._
- **Why does `Dong et al. 2024 - Ediacaran palaeo-ocean environment (Earth-Science Reviews)` connect `Ediacaran Geochemistry` to `Bayesian Seismic Inversion`?**
  _High betweenness centrality (0.028) - this node is a cross-community bridge._
- **What connects `VelocityGAN (GAN-based FWI)`, `Marmousi Velocity Model (2D seismic benchmark)`, `SEG Advanced Modeling Corporation (SEAM) Phase 1 Salt Model` to the rest of the system?**
  _42 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Bayesian Seismic Inversion` be split into smaller, more focused modules?**
  _Cohesion score 0.06 - nodes in this community are weakly interconnected._