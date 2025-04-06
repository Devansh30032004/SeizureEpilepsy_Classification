# 🧠 Seizure Epilepsy Classification using Quantum Convolutional Neural Network (QCNN)

This repository contains a project on classifying seizure (epileptic) activity from EEG signal data using an **8-qubit Quantum Convolutional Neural Network (QCNN)**.

## 🚀 Project Highlights

- ✅ **Model**: 8-qubit Quantum Convolutional Neural Network (QCNN)  
- 📉 **Dimensionality Reduction**: Applied **Autoencoders** on EEG signals  
- 🧪 **Training Strategy**: Used **cropped training** with EEG windows of **100/176 seconds**  
- 🎯 **Accuracy Achieved**: Up to **78%** on test data  
- 🧠 **EEG Data**: Sampled at **176 Hz**, pre-processed and segmented into ictal, preictal, and interictal states

## 🧬 Quantum Neural Network Model

The QCNN architecture was inspired by the tutorial from Qiskit Machine Learning.  
Refer to the detailed explanation here:  
🔗 [Quantum Convolutional Neural Networks - Qiskit Tutorial](https://qiskit-community.github.io/qiskit-machine-learning/tutorials/11_quantum_convolutional_neural_networks.html)

## 📁 Dataset Structure

The dataset consists of EEG `.mat` files organized as:

<pre> ## 📁 Dataset Structure The dataset is organized into the following folders: ``` EEG_epilepsy/ 
  ├── ictal/ # EEG data during seizure (label: y = 1) 
  ├── preictal/ # EEG data before seizure onset (label: y = 1) 
  └── interictal/ # EEG data between seizures (label: y = 0) 
  ``` Each `.mat` file contains 5.12 seconds of EEG signal data recorded at 176 Hz. </pre>


Each file contains **5.12 seconds** of EEG recording.

## 🛠️ Tech Stack

- Python  
- Qiskit Machine Learning  
- Scikit-learn  
- TensorFlow / PyTorch (for Autoencoders)  
- NumPy, SciPy  

## 📊 Results

| Metric     | Value  |
|------------|--------|
| Accuracy   | 78%    |
| Qubits     | 8      |
| Signal Seg | 100/176 sec |  
| Sampling Rate | 176 Hz |

---

## 📌 Future Improvements

- Explore hybrid classical-quantum models  
- Optimize autoencoder performance  
- Apply on real-time streaming EEG data  

---

## 🤝 Contribution

Feel free to fork, star ⭐, or raise an issue if you'd like to collaborate!

---

## 📜 License

This project is open-sourced under the MIT License.
