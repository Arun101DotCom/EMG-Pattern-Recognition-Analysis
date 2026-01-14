# EMG-Pattern-Recognition-Analysis
MSc Dissertation: Propose Optimal Conditions for EMG Pattern Recognition Systems by Comparing and Analysing with Various Conditions, Features, and Classifiers.
**MSc Dissertation | Newcastle University**

## 🔬 Project Overview
This research investigates the development of optimized myoelectric control systems for artificial prosthetic arms using the **NinaPro DB1 database**. The study identifies the most effective combinations of window sizes, filtering conditions, and signal features to achieve high-accuracy hand gesture recognition.

The project is structured into four research segments:
* **Part A:** General findings on windowing and filtering.
* **Part B:** Combined dataset analysis (27 Subjects).
* **Part C:** Individual subject analysis using statistical ranking.
* **Part D:** Development of a high-performance Hybrid Model.

## 🏆 Key Achievements
* **Peak Accuracy:** Achieved **97.10%** classification accuracy using Random Forest.
* **Statistical Rigor:** Applied the **Friedman non-parametric test** to rank features across 27 subjects.
* **Optimized Latency:** Identified the **250ms–500ms** window as the "Gold Standard" for balancing accuracy and real-time processing time.
* **Feature Discovery:** Identified **TF-Energy** (Time-Frequency Energy) as the most robust feature with an average rank of **1.22**.



## 🛠️ System Architecture & Hybrid Workflow
The system utilizes a hybrid software approach to leverage the best tools for Signal Processing and Machine Learning:

1. **MATLAB Pipeline:** Used for data preprocessing, digital filtering (MSE/SNR analysis), and complex feature extraction (Time, Frequency, and Time-Frequency domains).
2. **Python Pipeline:** Utilized for Machine Learning model training (LDA, SVM, KNN, Random Forest, ANN), hyperparameter tuning, and real-time classification benchmarking.



## 📊 Detailed Experimental Results

### **1. Feature Engineering Tiers**
Through mean, median, and standard deviation analysis, features were categorized by their information density:
* **Tier 1 (Best):** SSC, WL, TP, TF-Energy.
* **Tier 2 (Moderate):** WAMP, RMS, MNF, MDF, PSD.
* **Tier 3 (Least Informative):** MAV, VAR, ZC, PF.

### **2. Classifier Performance**
| Model | Accuracy Range | Notes |
| **Random Forest** | **85.37% - 97.10%** | Best overall accuracy and F1-score. |
| **KNN** | High Consistency | Best for low-latency computation. |
| **Hybrid Model** | **90.49% (Avg)** | Integrated Time/Freq/T-Freq domains for robust prediction. |

## 📂 Repository Structure (Research Workflow)
To navigate the research methodology, please follow the folders in numerical order:

* **01_NinaPro_Dataset_DB1**: Documentation and source links for the raw sEMG signals of 27 subjects.
* **02_Matlab-Data_Preprocessing**: Scripts for digital filtering, windowing experiments (benchmarking 50-25ms through 800-400ms), and SNR/MSE calculations.
* **03_Feature_Extracted_dataset**: Processed datasets categorized by information density (Best, Moderate, and Least informative).
* **04_Python-Machine_Learning_Models**: Implementation of KNN, Random Forest, ANN, LDA, SVM and the Hybrid Model for hand pattern classification.
* **05_Technical_report**: The full MSc Dissertation PDF detailing all experimental targets and final conclusions.
* **06_key_findings**: A concise summary PDF highlighting the most significant results, optimal windowing parameters, and the 97.10% accuracy achievement.

**Author:** Arun Chakkyadath Chandran
**Institution:** Newcastle University, UK  
**Keywords:** Electromyography (EMG), Digital Signal Processing (DSP), Machine Learning, Random Forest, TinyML.

