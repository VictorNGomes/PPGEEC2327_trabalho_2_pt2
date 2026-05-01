# Graph Report - ./papers  (2026-04-29)

## Corpus Check
- 19 files · ~223,057 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 107 nodes · 149 edges · 10 communities detected
- Extraction: 78% EXTRACTED · 13% INFERRED · 9% AMBIGUOUS · INFERRED: 19 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Physics-Guided FWI|Physics-Guided FWI]]
- [[_COMMUNITY_VMB Uncertainty|VMB Uncertainty]]
- [[_COMMUNITY_OpenFWI Benchmarks|OpenFWI Benchmarks]]
- [[_COMMUNITY_Seismic Interpretation|Seismic Interpretation]]
- [[_COMMUNITY_3D FWI and Statics|3D FWI and Statics]]
- [[_COMMUNITY_GAN Seismic Processing|GAN Seismic Processing]]
- [[_COMMUNITY_Scalable 3D Architectures|Scalable 3D Architectures]]
- [[_COMMUNITY_Out-of-Scope Scene Flow|Out-of-Scope Scene Flow]]
- [[_COMMUNITY_Out-of-Scope Geochemistry|Out-of-Scope Geochemistry]]
- [[_COMMUNITY_GPS Deformation Outlier|GPS Deformation Outlier]]

## God Nodes (most connected - your core abstractions)
1. `Seismic Inversion Approaches for Reservoir Characterization` - 12 edges
2. `OPEN FWI: Large-scale Multi-structural Benchmark Datasets for Full Waveform Inversion` - 8 edges
3. `Synergizing Deep Learning and Full-waveform Inversion: Bridging Data-driven and Theory-guided Approaches for Enhanced Seismic Imaging` - 8 edges
4. `Physics-Guided Data-Driven Seismic Inversion: Recent Progress and Future Opportunities in Full-Waveform Inversion` - 7 edges
5. `An Empirical Study of Large-scale Data-driven Full Waveform Inversion` - 7 edges
6. `OpenFWI Benchmark Dataset Collection` - 7 edges
7. `Velocity Model Building` - 7 edges
8. `Uncertainty Quantification` - 7 edges
9. `Reflection Residual Statics Estimated Using a High-Resolution Neural Network` - 6 edges
10. `Current State and Future Directions for Deep Learning Based Automatic Seismic Fault Interpretation` - 6 edges

## Surprising Connections (you probably didn't know these)
- `Point-Voxel Correlation Fields` --semantically_similar_to--> `Physics-Informed Summary Statistics`  [AMBIGUOUS] [semantically similar]
  papers/cluster_B_VelocityModelBuilding/B4_Alkhalifah et al._2021.pdf → papers/cluster_B_VelocityModelBuilding/B5_Orozco et al._2024.pdf
- `B1 Chen et al. 2021 Unreadable Sign-In Placeholder` --conceptually_related_to--> `Velocity Model Building`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B1_Chen et al._2021.pdf → papers/cluster_B_VelocityModelBuilding/B3_AlAli & Anifowose_2022.pdf
- `GPS Deformation Modeling` --conceptually_related_to--> `Velocity Model Building`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B2_Geng et al._2022.pdf → papers/cluster_B_VelocityModelBuilding/B3_AlAli & Anifowose_2022.pdf
- `Scene Flow Estimation from Point Clouds` --conceptually_related_to--> `Velocity Model Building`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B4_Alkhalifah et al._2021.pdf → papers/cluster_B_VelocityModelBuilding/B3_AlAli & Anifowose_2022.pdf
- `VelocityGAN` --conceptually_related_to--> `Generative Models for Deep-learning FWI`  [AMBIGUOUS]
  papers/cluster_A_FWI_DeepLearning/A1_Deng et al._2022.pdf → papers/cluster_A_FWI_DeepLearning/A6_Zerafa et al._2025.pdf

## Hyperedges (group relationships)
- **OpenFWI Benchmark Ecosystem** — paper_a1_deng_et_al_2022_openfwi, dataset_openfwi, dataset_openfwi_twelve_datasets_2_1tb, method_inversionnet, method_velocitygan, method_upfwi, method_inversionnet3d, claim_openfwi_enables_reproducible_benchmarking [EXTRACTED 0.90]
- **Physics-guided FWI Methods** — method_physics_guided_machine_learning, method_pinns, method_physics_guided_deep_autoencoder, method_upfwi, task_full_waveform_inversion [INFERRED 0.84]
- **Large-scale OpenFWI Empirical Study** — paper_a4_jin_et_al_2024_big_data_fwi, dataset_openfwi_ten_2d_subsets_470k_pairs, method_bigfwi_training, method_inversionnet, claim_big_data_improves_fwi_generalization, claim_model_capacity_must_scale_with_data_size [EXTRACTED 0.92]
- **Deep-learning FWI Challenges and Future Work** — paper_a6_zerafa_et_al_2025_deep_learning_fwi_review, limitation_data_quality_and_generalization, limitation_model_complexity, future_direction_hybrid_models, future_direction_generative_models, future_direction_uncertainty_quantification [EXTRACTED 0.88]
- **Cluster B Velocity Model Building Core** — paper_b3_alali_anifowose_2022_seismic_velocity_modeling_ml_review, paper_b5_orozco_erdinc_zeng_louboutin_herrmann_2024_ml_vmb_uq, concept_velocity_model_building, concept_full_waveform_inversion, concept_machine_learning_for_velocity_modeling, concept_uncertainty_quantification [INFERRED 0.86]
- **Diffusion Bayesian VMB UQ Workflow** — paper_b5_orozco_erdinc_zeng_louboutin_herrmann_2024_ml_vmb_uq, concept_diffusion_networks, concept_physics_informed_summary_statistics, concept_subsurface_offset_image_gathers, concept_bayesian_posterior_velocity_models, concept_uncertainty_quantification [EXTRACTED 0.94]
- **ML-Assisted Velocity Estimation Modes** — paper_b3_alali_anifowose_2022_seismic_velocity_modeling_ml_review, concept_nmo_velocity_picking, concept_fwi_convergence_assistance, concept_machine_learning_for_velocity_modeling, concept_poor_starting_model_cycle_skipping [EXTRACTED 0.90]
- **Cluster B Source Quality Mismatch Set** — paper_b1_chen_et_al_2021_unreadable_sign_in_placeholder, paper_b2_cosenza_muralles_demets_et_al_colima_jalisco_gps_deformation, paper_b4_wei_wang_rao_lu_zhou_2021_pv_raft_scene_flow, concept_source_quality_mismatch, concept_source_quality_mismatches [INFERRED 0.82]
- **GAN-Based Seismic Processing Tasks** — paper_c1_kaur_et_al_2021_ground_roll_attenuation, paper_c3_zhang_et_al_2022_gan_interpolation, concept_generative_adversarial_networks, concept_ground_roll_attenuation, concept_seismic_data_interpolation [INFERRED 0.86]
- **Preprocessing Chain for Improved Seismic Imaging** — concept_ground_roll_attenuation, concept_seismic_data_interpolation, concept_residual_statics, concept_seismic_imaging, concept_migration_imaging_workflow [INFERRED 0.78]
- **Deep Learning Residual Statics Estimation** — paper_c4_wang_et_al_2022_residual_statics, concept_residual_statics, concept_high_resolution_neural_network, concept_surface_consistent_corrections, concept_stack_power_maximization, concept_normal_moveout_correction [EXTRACTED 0.90]
- **Scalable InversionNet3D Architecture for 3D FWI** — paper_c5_zeng_et_al_2022_inversionnet3d, concept_inversionnet3d, concept_3d_full_waveform_inversion, concept_encoder_decoder_network, concept_group_convolution, concept_invertible_layers, concept_scalable_deep_learning_architectures, concept_kimberlina_3d_dataset [EXTRACTED 0.93]
- **Deep Learning Fault Interpretation Review Stack** — paper_d1_an_2023_fault_interpretation_review, concept_automatic_seismic_fault_interpretation, concept_deep_learning_for_fault_interpretation, concept_convolutional_neural_networks, concept_u_net_fault_segmentation, concept_annotated_fault_data_gap [EXTRACTED 0.92]
- **Reservoir Characterization Inversion Family** — paper_d3_li_2023_reservoir_inversion_review, concept_seismic_inversion, concept_reservoir_characterization, concept_avo_inversion, concept_full_waveform_inversion, concept_inverse_rock_physics [EXTRACTED 0.93]
- **Uncertainty-Aware Seismic Inversion Methods** — paper_d3_li_2023_reservoir_inversion_review, concept_uncertainty_quantification, concept_bayesian_inversion, concept_ensemble_kalman_filter, concept_seismic_inversion [EXTRACTED 0.86]
- **Cluster D Source Quality Issues** — paper_d2_dong_2024_ediacaran_geochemistry, paper_d3_li_2023_reservoir_inversion_review, paper_d4_zhao_2021_reservoir_inversion_review_duplicate, concept_source_quality_mismatch, concept_duplicate_reservoir_inversion_content [INFERRED 0.78]

## Communities

### Community 0 - "Physics-Guided FWI"
Cohesion: 0.09
Nodes (25): Physics-guided Autoencoder Removes Need for Starting Velocity Model, Physics-guided Autoencoder Produces Robust Results under Noise and Complex Salt Bodies, PINNs Handle Wave-equation Boundary Conditions and Limited Surface Data, Marmousi Synthetic Model, SEG Advanced Modeling Corporation Phase 1 Salt Model, Generative Models for Deep-learning FWI, Hybrid Deep-learning and Physics-based FWI Models, Uncertainty Quantification for Deep-learning FWI (+17 more)

### Community 1 - "VMB Uncertainty"
Cohesion: 0.15
Nodes (17): Bayesian Inversion, Bayesian Posterior Samples for Migration Velocity Models, Diffusion Networks, Ensemble Kalman Filter, Field Dataset Scalability, Full-Waveform Inversion, FWI Convergence Assistance, Machine Learning for Velocity Modeling (+9 more)

### Community 2 - "OpenFWI Benchmarks"
Cohesion: 0.16
Nodes (16): Large-scale Combined Training Improves FWI Accuracy and Generalization, Model Capacity Must Scale with FWI Data Size, OpenFWI Enables Diversified Rigorous Reproducible FWI Benchmarking, 3D Kimberlina-V1 Dataset, OpenFWI Benchmark Dataset Collection, OpenFWI 10 2D Subsets with 470K Seismic-Velocity Pairs, OpenFWI 12-dataset 2.1TB Synthetic Corpus, BigFWI Combined-dataset Training (+8 more)

### Community 3 - "Seismic Interpretation"
Cohesion: 0.2
Nodes (15): Annotated Fault Data Gap, Automatic Seismic Fault Interpretation, AVO Inversion, Convolutional Neural Networks, Deep Learning for Fault Interpretation, Duplicate Reservoir Inversion Content, Inverse Rock Physics, Reservoir Characterization (+7 more)

### Community 4 - "3D FWI and Statics"
Cohesion: 0.25
Nodes (11): 3D Full Waveform Inversion, Encoder-Decoder Network, High-Resolution Neural Network, Normal Moveout Correction, Residual Statics, Seismic Imaging, Stack Power Maximization, Surface-Consistent Corrections (+3 more)

### Community 5 - "GAN Seismic Processing"
Cohesion: 0.42
Nodes (9): Generative Adversarial Networks, Ground-Roll Attenuation, Local Time-Frequency Transform, Migration and Imaging Workflow, Missing Trace Reconstruction, Regularized Non-Stationary Regression, Seismic Data Interpolation, Seismic Ground-Roll Noise Attenuation Using Deep Learning (+1 more)

### Community 6 - "Scalable 3D Architectures"
Cohesion: 0.5
Nodes (5): Group Convolution, InversionNet3D, Invertible Layers, 3D Kimberlina Dataset, Scalable Deep Learning Architectures

### Community 7 - "Out-of-Scope Scene Flow"
Cohesion: 0.5
Nodes (4): Point-Voxel Correlation Fields, Scene Flow Estimation from Point Clouds, Source-Quality Mismatches in Cluster B, PV-RAFT: Point-Voxel Correlation Fields for Scene Flow Estimation of Point Clouds

### Community 8 - "Out-of-Scope Geochemistry"
Cohesion: 0.67
Nodes (3): Ediacaran Palaeo-Ocean Environment, Isotope Geochemistry, The Ediacaran Palaeo-Ocean Environment in the Northwest Margin of South China Craton

### Community 9 - "GPS Deformation Outlier"
Cohesion: 1.0
Nodes (2): GPS Deformation Modeling, Co-Seismic and Post-Seismic Deformation for the 1995 Colima-Jalisco and 2003 Tecoman Earthquakes

## Ambiguous Edges - Review These
- `OPEN FWI: Large-scale Multi-structural Benchmark Datasets for Full Waveform Inversion` → `A1 Weak Title Metadata Captured as Affiliation and Email Block`  [AMBIGUOUS]
  papers/cluster_A_FWI_DeepLearning/A1_Deng et al._2022.pdf · relation: rationale_for
- `Physics-informed Neural Networks (PINNs) for Wave Propagation and Full Waveform Inversions` → `A3 Weak Title Metadata Captured as Affiliation Block`  [AMBIGUOUS]
  papers/cluster_A_FWI_DeepLearning/A3_Rasht-Behesht et al._2022.pdf · relation: rationale_for
- `Synergizing Deep Learning and Full-waveform Inversion: Bridging Data-driven and Theory-guided Approaches for Enhanced Seismic Imaging` → `A6 Weak Title Metadata Captured as Author Contact Block`  [AMBIGUOUS]
  papers/cluster_A_FWI_DeepLearning/A6_Zerafa et al._2025.pdf · relation: rationale_for
- `VelocityGAN` → `Generative Models for Deep-learning FWI`  [AMBIGUOUS]
  papers/cluster_A_FWI_DeepLearning/A6_Zerafa et al._2025.pdf · relation: conceptually_related_to
- `B1 Chen et al. 2021 Unreadable Sign-In Placeholder` → `Velocity Model Building`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B1_Chen et al._2021.pdf · relation: conceptually_related_to
- `Velocity Model Building` → `GPS Deformation Modeling`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B2_Geng et al._2022.pdf · relation: conceptually_related_to
- `Velocity Model Building` → `Scene Flow Estimation from Point Clouds`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B4_Alkhalifah et al._2021.pdf · relation: conceptually_related_to
- `Physics-Informed Summary Statistics` → `Point-Voxel Correlation Fields`  [AMBIGUOUS]
  papers/cluster_B_VelocityModelBuilding/B4_Alkhalifah et al._2021.pdf · relation: semantically_similar_to
- `Source Quality or Cluster Mismatch` → `The Ediacaran Palaeo-Ocean Environment in the Northwest Margin of South China Craton`  [AMBIGUOUS]
  papers/cluster_D_SeismicInterpretation/D2_Wu et al._2024.pdf · relation: rationale_for
- `Source Quality or Cluster Mismatch` → `Seismic Inversion Approaches for Reservoir Characterization`  [AMBIGUOUS]
  papers/cluster_D_SeismicInterpretation/D3_Li et al._2023.pdf · relation: conceptually_related_to
- `Source Quality or Cluster Mismatch` → `Seismic Inversion Approaches for Reservoir Characterization Duplicate Entry`  [AMBIGUOUS]
  papers/cluster_D_SeismicInterpretation/D4_Zhao et al._2021.pdf · relation: conceptually_related_to
- `Generative Adversarial Networks` → `InversionNet3D`  [AMBIGUOUS]
  papers/cluster_C_RTM_Migration/C5_Zeng et al._2022.pdf · relation: conceptually_related_to
- `3D Full Waveform Inversion` → `Migration and Imaging Workflow`  [AMBIGUOUS]
  papers/cluster_C_RTM_Migration/C5_Zeng et al._2022.pdf · relation: conceptually_related_to
- `The Ediacaran Palaeo-Ocean Environment in the Northwest Margin of South China Craton` → `Reservoir Characterization`  [AMBIGUOUS]
  papers/cluster_D_SeismicInterpretation/D2_Wu et al._2024.pdf · relation: conceptually_related_to

## Knowledge Gaps
- **34 isolated node(s):** `Cycle-skipping`, `Ill-posed Seismic Inversion`, `OpenFWI 12-dataset 2.1TB Synthetic Corpus`, `Marmousi Synthetic Model`, `SEG Advanced Modeling Corporation Phase 1 Salt Model` (+29 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `GPS Deformation Outlier`** (2 nodes): `GPS Deformation Modeling`, `Co-Seismic and Post-Seismic Deformation for the 1995 Colima-Jalisco and 2003 Tecoman Earthquakes`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `OPEN FWI: Large-scale Multi-structural Benchmark Datasets for Full Waveform Inversion` and `A1 Weak Title Metadata Captured as Affiliation and Email Block`?**
  _Edge tagged AMBIGUOUS (relation: rationale_for) - confidence is low._
- **What is the exact relationship between `Physics-informed Neural Networks (PINNs) for Wave Propagation and Full Waveform Inversions` and `A3 Weak Title Metadata Captured as Affiliation Block`?**
  _Edge tagged AMBIGUOUS (relation: rationale_for) - confidence is low._
- **What is the exact relationship between `Synergizing Deep Learning and Full-waveform Inversion: Bridging Data-driven and Theory-guided Approaches for Enhanced Seismic Imaging` and `A6 Weak Title Metadata Captured as Author Contact Block`?**
  _Edge tagged AMBIGUOUS (relation: rationale_for) - confidence is low._
- **What is the exact relationship between `VelocityGAN` and `Generative Models for Deep-learning FWI`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `B1 Chen et al. 2021 Unreadable Sign-In Placeholder` and `Velocity Model Building`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Velocity Model Building` and `GPS Deformation Modeling`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Velocity Model Building` and `Scene Flow Estimation from Point Clouds`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._