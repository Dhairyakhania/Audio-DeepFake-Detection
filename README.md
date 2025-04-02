# Audio Deepfake Detection

## Overview
This repository contains an implementation of an audio deepfake detection system using machine learning techniques. The project explores feature extraction from audio signals and classification using models like XGBoost and Support Vector Machine (SVM) with an RBF kernel.

## Features
- **Feature Extraction:**
  - Linear Predictive Coding (LPC)
  - Mel-Frequency Cepstral Coefficients (MFCCs)
  - Zero Crossing Rate (ZCR)
  - Spectral Features (centroid, bandwidth, contrast, roll-off)
  - Harmonics-to-Noise Ratio (HNR)
  - Formants
- **Machine Learning Models:**
  - XGBoost Classifier
  - SVM with RBF Kernel
- **Dataset Used:**
  - [ASVspoof 5](https://zenodo.org/records/14498691)
- **Prediction Function:** Classifies audio samples as "Spoof" (deepfake) or "Bonafide" (real speech)

## Installation
### Prerequisites
Ensure you have Python installed along with the necessary dependencies.
```bash
pip install -r requirements.txt
```

## Usage

## How to Run the Notebook
1. Clone this repository:
   ```bash
   git clone https://github.com/Dhairyakhania/Audio-DeepFake-Detection.git
   ```
2. Navigate to the project folder:
   ```bash
   cd Audio-DeepFake-Detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
   Then, open `audio_deepFake_detection.ipynb` and run all cells.

## Results
- XGBoost performed well in handling high-dimensional feature space and provided interpretability through feature importance.
- SVM with RBF Kernel effectively captured complex feature distributions.
- Feature extraction played a crucial role; missing values led to sample rejection.

## Future Improvements
- Implement deep learning approaches (CNNs, RNNs) for better accuracy.
- Expand feature set to include phase-based features.
- Optimize hyperparameters for improved classification.

## Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References
1. [ASVspoof 5 Dataset](https://zenodo.org/records/14498691)
2. [Media-Sec Lab Audio Deepfake Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection)
