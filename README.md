# Comparative Analysis and Deep Learning Approaches for ECG-Derived Respiration Signal Estimation using the Fantasia Dataset

This project aims to establish robust baselines for ECG-derived respiration signal analysis using well-established signal processing methods and compare these with deep learning solutions. The Fantasia dataset, containing long-term ECG recordings from healthy young and elderly subjects, was used for this purpose.

### Key Components of the Project:

1. **Introduction**: Discusses the importance of robust baselines in ECG-derived respiration signal analysis and introduces the Fantasia dataset.

2. **Dataset Description**: Details about the Fantasia dataset, including:
   - Number of Subjects: 40 (20 young, 20 elderly)
   - Ages: Young subjects (21-34 years), Elderly subjects (68-85 years)
   - Conditions: Healthy
   - Sampling Frequency: 250 Hz
   - Duration: 120 minutes

3. **Performance of Signal Processing Methods**: Evaluates traditional signal processing algorithms using Mean Squared Error (MSE) and Mean Cross-Correlation (CC) metrics.

4. **Deep Learning Methods**: Explores deep learning approaches for extracting respiratory signals from ECG data, highlighting models like RespNet.

5. **Results**:
   - **Model Architecture**: Implements a fully convolutional autoencoder network inspired by the U-Net model, comprising convolutional layers, ReLU activations, Batch Normalization, MaxPooling, and up-sampling techniques.
   - **Evaluation**: Describes the preprocessing steps, cross-validation technique, and metrics used for model evaluation.
   - **Results**: Presents the performance results, showing the deep learning method's average validation CC of 0.51 and MSE of 0.046, outperforming 4 out of 6 traditional signal processing algorithms.
  
6. **Comparison**:

**Mean Cross Correlation (CC)**
The deep learning method outperforms 4 out of 6 traditional signal processing algorithms:
- ELF_RSlinB_FMebw_FPt_RDtGC_EHF: by 0.0114 (2.29% improvement)
- flt_BFi: by 0.1396 (37.7% improvement)
- flt_Wam: by 0.1228 (31.7% improvement)
- flt_Wfm: by 0.0615 (13.7% improvement)

The deep learning method falls short of 2 algorithms:
- ELF_RSlinB_FMeam_FPt_RDtGC_EHF: by 0.0759 (12.9% lower)
- ELF_RSlinB_FMefm_FPt_RDtGC_EHF: by 0.0453 (8.9% lower)

**Mean Squared Error (MSE)**
The deep learning method outperforms all 6 traditional signal processing algorithms:
- ELF_RSlinB_FMeam_FPt_RDtGC_EHF: by 0.0260 (36.1% improvement)
- ELF_RSlinB_FMebw_FPt_RDtGC_EHF: by 0.0238 (34.1% improvement)
- ELF_RSlinB_FMefm_FPt_RDtGC_EHF: by 0.0246 (34.8% improvement)
- flt_BFi: by 0.0379 (45.2% improvement)
- flt_Wam: by 0.0474 (50.7% improvement)
- flt_Wfm: by 0.0361 (44.0% improvement)



7. **Conclusion**: 
The deep learning approach demonstrates superior performance in reducing error (MSE) across all comparisons and improves correlation (CC) in the majority of cases compared to traditional signal processing methods. This highlights the potential of deep learning models to surpass traditional methods in complex biosignal analysis tasks, paving the way for improved diagnostic and monitoring capabilities in healthcare.
