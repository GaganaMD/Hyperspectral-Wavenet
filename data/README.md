# Data Description

This project utilizes both synthetic and real-world hyperspectral datasets to evaluate the performance and robustness of the proposed model. Below is an overview of the datasets:

## Synthetic Datasets
The synthetic datasets were designed to simulate ideal conditions for hyperspectral data analysis.

- **SyntheticImage**:  
  - **Shape**: `(128, 128, 431)`  
  - **Description**: A hyperspectral cube where each pixel is a linear combination of predefined endmembers from the `endmembersGT` matrix.  
  - **Purpose**: Used for controlled testing and validation of the model under idealized conditions.  

- **Ground Truth Data**:  
  - **`endmembersGT`**: Contains the known endmember signatures.  
  - **`abundanciesGT`**: Corresponding abundance maps for each pixel in the synthetic image.  
  - **Usage**: These serve as references for quantitative analysis using metrics such as:
    - Root Mean Square Error (RMSE)  
    - Spectral Angle Distance (SAD)  
    - Spectral Information Divergence (SID)  

### Key Features
- Provides a controlled environment free from external noise or non-linear mixing effects.  
- Enables precise performance evaluation of the model.

---

## Real-World Dataset
The real-world dataset captures hyperspectral data in practical conditions with environmental complexities.

- **Dataset Details**:  
  - **Shape**: `(307, 307, 162)`  
  - **Spatial Resolution**: 307 × 307 pixels.  
  - **Spectral Bands**: 162.  

- **Characteristics**:  
  - Includes real-world spectral variability caused by environmental factors.  
  - Contains noise, atmospheric disturbances, and potential artifacts.  

- **Purpose**:  
  - Used to assess the robustness and generalizability of the model in realistic scenarios.

### Key Features
- Simulates real-world challenges for hyperspectral image analysis.  
- Tests the model's ability to handle noise and non-linear mixing.

---

## Summary
By experimenting on both synthetic datasets with well-defined ground truths and real-world datasets with inherent complexities, this project ensures that the proposed model is validated across both idealized and practical conditions.
