# Hyperspectral Dataset Overview

This project utilizes both synthetic and real-world hyperspectral datasets to evaluate the performance and robustness of the proposed model. Below is a detailed description of the datasets and their characteristics:

---

## Synthetic Datasets

The synthetic datasets are crafted to simulate ideal conditions for hyperspectral data analysis, providing a controlled environment for testing and validation.

### **1. Synthetic Image**
- **Shape**: `(128, 128, 431)`  
- **Description**: A hyperspectral cube where each pixel is a linear combination of predefined endmembers from the `endmembersGT` matrix.  
- **Purpose**: Serves as a testbed for evaluating the model under idealized conditions.  

### **2. Ground Truth Data**
- **`endmembersGT`**: Contains predefined endmember signatures.  
- **`abundanciesGT`**: Corresponding abundance maps for each pixel in the synthetic image.  

#### **Usage**
The ground truth data facilitates quantitative evaluation of the model using the following metrics:
- **Root Mean Square Error (RMSE)**: Measures the error between predicted and true values.  
- **Spectral Angle Distance (SAD)**: Quantifies the angular difference between predicted and actual spectra.  
- **Spectral Information Divergence (SID)**: Assesses spectral dissimilarity based on divergence.  

#### **Key Features**
- Provides a noise-free, controlled environment.  
- Enables precise evaluation of the model’s performance without interference from external factors such as noise or non-linear mixing effects.  

---

## Real-World Dataset

The real-world dataset introduces practical complexities and environmental variabilities for hyperspectral data analysis.

### **Dataset Details**
- **Shape**: `(307, 307, 162)`  
- **Spatial Resolution**: 307 × 307 pixels.  
- **Spectral Bands**: 162.  

### **Characteristics**
- Incorporates spectral variability due to environmental factors.  
- Includes real-world challenges such as noise, atmospheric disturbances, and potential artifacts.  

### **Purpose**
This dataset tests the model’s ability to:
- Handle real-world noise and spectral variability.  
- Demonstrate robustness and generalizability under non-ideal conditions.  

#### **Key Features**
- Simulates real-world complexities for hyperspectral image analysis.  
- Evaluates the model’s ability to process noisy and non-linearly mixed data.  

---

## Summary

This dual-dataset approach ensures comprehensive validation of the proposed model:
- The **synthetic datasets** provide a benchmark for performance evaluation under controlled conditions.  
- The **real-world dataset** assesses the model’s resilience and effectiveness in practical scenarios.  

### **Data Access**
The datasets can be accessed via the following link:  
[Google Drive - Hyperspectral Datasets](https://drive.google.com/drive/folders/1ffHf5ageSOwfZbnas5O2MtvtTDUhygZk)

