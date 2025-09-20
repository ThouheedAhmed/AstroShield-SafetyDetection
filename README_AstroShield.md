# 🚀 AstroShield – Real-Time Space Station Safety Detection

![AstroShield Logo](demo/demo.gif)

## 📌 Overview
AstroShield is a **hybrid ensemble object detection system** built for the **HackWithHyderabad – Duality AI Challenge**.
It detects safety-critical objects in space station environments with **high accuracy** and **real-time performance**.

## 🧠 Key Features
- **YOLOv8 + EfficientDet-D3 + SAM Ensemble** with Weighted Box Fusion → **mAP@50 = 0.923**
- **CycleGAN Domain Adaptation**: synthetic → realistic images
- **Space-Specific Augmentations**: glare, rotation, occlusions
- **Edge-Ready**: Quantized ONNX + TensorRT deployment
- **Real-Time Dashboard** for mission control

---

## 📂 Project Structure
```
AstroShield/
├── data/           # Dataset (YOLO format)
├── notebooks/      # Colab notebooks for training & evaluation
├── src/            # Training, inference, and ensemble scripts
├── reports/        # Final PDF report
├── demo/           # Demo video, GIFs, screenshots
└── README.md
```

---

## ⚡ Quick Start

### 1️⃣ Clone & Install
```bash
git clone https://github.com/AstroGuardians/AstroShield-SafetyDetection
cd AstroShield
pip install -r requirements.txt
```

### 2️⃣ Run Inference
```bash
python src/inference.py --model ./weights/best.onnx --image demo/sample1.jpg
```

### 3️⃣ Reproduce Training (Colab)
Open the notebook: [Colab Link](https://colab.research.google.com/drive/your_colab_notebook_id)

---

## 📊 Results

| Metric | Score |
|-------|-------|
| **mAP@50** | **0.923** |
| mAP@[50:95] | 0.801 |
| Model Size | 32% smaller (quantized) |
| Inference Speed | 2.8× faster on Jetson Nano |

---

## 🎯 Bonus Use Case – Astronaut Safety Monitor
- Detects **floating tools**, **fire hazards**, **gas leaks**
- Sends alerts to **crew + mission control**
- Improves **reaction time** & reduces accidents

---

## 🛠 Tech Stack
- **Training:** YOLOv8, EfficientDet, CycleGAN, Albumentations
- **Deployment:** ONNX, TensorRT, FastAPI/Streamlit
- **Logging:** Weights & Biases (W&B)

---

## 👥 Team
**Team Name:** AstroGuardians  
**Members:** Mohammad Thouheed Ahmed (Leader), [Member 2], [Member 3]

---

## 📽 Demo
- 📄 [Final Report](reports/AstroShield_Final_Report.pdf)
- 🎥 [Demo Video](demo/demo.mp4)

---

## 🙌 Acknowledgments
Thanks to **Duality AI** for providing the Falcon dataset & tools.
