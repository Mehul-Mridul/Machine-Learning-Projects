## **🫀 NRC-Net: Noise-Robust Cardio Net for Heart Sound Classification**

### **🔍 Overview**
NRC-Net is a lightweight and efficient **Deep Learning model** designed to classify **heart sounds** and detect valvular cardiac diseases, even in the presence of **noisy environments**. This model utilizes **Continuous Wavelet Transform (CWT)** as the optimal transformation method and achieves an accuracy of **86%** on our trained dataset.

Inspired by the research paper **["NRC-Net: Automated Noise Robust Cardio Net for Detecting Valvular Cardiac Diseases"](https://doi.org/10.1016/j.bspc.2023.105272)**, we trained and fine-tuned NRC-Net on a heart sound dataset to improve real-world applicability in medical diagnostics.

---

## **📌 Features**
✅ **Lightweight Model** - Optimized for efficiency while maintaining high accuracy.  
✅ **Noise-Robust** - Can classify heart conditions despite ambient noise interference.  
✅ **Deep Learning Powered** - Uses a combination of **Convolutional Neural Networks (CNN)** and **Recurrent Neural Networks (RNN)**.  
✅ **Attention Mechanism** - Incorporates an **Attention Block** for better feature extraction.  
✅ **Medical Applicability** - Can assist in early **Cardiovascular Disease (CVD)** detection, particularly in **low-resource settings**.

---

## **📚 Dataset**
We trained **NRC-Net** on a **Heart Sound Dataset** consisting of five heart sound categories:  
🔹 **Mitral Regurgitation (MR)**  
🔹 **Aortic Stenosis (AS)**  
🔹 **Mitral Stenosis (MS)**  
🔹 **Mitral Valve Prolapse (MVP)**  
🔹 **Normal Heart Sounds (N)**  

### **Data Preprocessing**  
✔ **Bandpass filtering** (50Hz - 800Hz)  
✔ **Resampling** (2000Hz)  
✔ **Noise Augmentation** (Lung sound & AWGN noise at various SNRs)  

---

## **🛠️ Model Architecture**
NRC-Net is built using a combination of **CNN & RNN** layers with attention-based feature extraction:

### **🏢 Architecture Components**
1️⃣ **Spatial Feature Extractor Block (SFEB)** - Extracts spatial features using CNN layers.  
2️⃣ **Holistic Attention Block (HAB)** - Highlights important features using channel-wise attention.  
3️⃣ **Temporal Feature Extractor Block (TFEB)** - Captures sequential dependencies using LSTMs.  
4️⃣ **Terminal Classification Block (TCB)** - Final dense layers for classification.  

---

## **🚀 Performance**
📊 **Accuracy**: **86%** (on our dataset)  
📉 **Robustness to Noise**: NRC-Net performs well even under **noisy heart sound conditions**.  
🏆 **Optimized for Deployment**: Lower computational overhead compared to traditional deep networks.  

---

## **🗂 How to Run**
### **🖥️ Requirements**
```
Python 3.8+
TensorFlow / PyTorch
NumPy
Matplotlib
Librosa (for audio processing)
```

### **🔧 Installation**
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/NRC-Net.git
cd NRC-Net
pip install -r requirements.txt
```

### **📝 Training the Model**
```python
python train.py --epochs 50 --batch_size 16
```

### **🔎 Running Inference**
```python
python predict.py --audio_path sample.wav
```

---

## **📖 Research Paper Credit**
This project is heavily inspired by:  
📝 **["NRC-Net: Automated Noise Robust Cardio Net for Detecting Valvular Cardiac Diseases"](https://doi.org/10.1016/j.bspc.2023.105272)**  
Published in *Biomedical Signal Processing and Control (2023)*.

We acknowledge the authors for their research and methodologies, which helped in shaping this project.

---

## **🔮 Future Improvements**
🔹 **Enhancing Model Accuracy** - Fine-tuning NRC-Net for even higher classification accuracy.  
🔹 **Deploying in Medical Applications** - Integration with real-world **digital stethoscopes**.  
🔹 **Explainability with GradCAM** - Improving interpretability for **medical professionals**.  
🔹 **Handling More Noise Sources** - Adding robustness to **hospital ambient noises**.  

---

## **👨‍💻 Contributors**
💡 **Mehul Mridul** - Core Developer  
💡 **Ahhsan Hoque**  
💡 **Saatvik Krishna Vaish**  

---

## **🗃️ License**
This project is licensed under the **MIT License**.


