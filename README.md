# Establishing Baselines for Deep Learning Approaches in ECG-Derived Respiration Signal Analysis on Fantasia Dataset

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

6. **Conclusion**: Summarizes the findings, emphasizing the effectiveness of the deep learning approach and outlining future work to explore different architectures and datasets for improved results.

This project highlights the potential of deep learning models to surpass traditional methods in complex biosignal analysis tasks, paving the way for improved diagnostic and monitoring capabilities in healthcare.
