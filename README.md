# FaceID-Pipeline: Clustering to Multi-Face Classification  
A modular pipeline for face recognition — from unsupervised clustering to real-time multi-face detection with Gradio.

---
## 🧠 Project Overview

This project builds a complete facial recognition pipeline that progresses through four modular phases — starting with unsupervised face clustering and culminating in real-time multi-face classification using interactive Gradio apps.

The pipeline is designed to simulate a real-world facial recognition workflow, where raw face images are first clustered without labels, then used to train a classifier, and finally deployed in apps that can detect and classify faces in both single and group images.

We begin by generating face embeddings using a pre-trained model, then apply clustering algorithms to group similar faces. These clusters are manually labeled and used to train a FastAI-based classifier. The trained model is then integrated into two Gradio apps — one for single-face classification and another for multi-face detection and classification.

✅ The entire pipeline — from data preprocessing and clustering to model training and app deployment — is modularized across four Jupyter notebooks.  
✅ Built using **FastAI**, **Gradio**, and **face_recognition** libraries for a clean and reproducible ML workflow.

🧪 Evaluation is conducted qualitatively by testing the classifier on unseen face images and assessing its ability to correctly identify individuals across varied lighting, angles, and group compositions.

📊 The full pipeline includes:

- Face embedding generation and clustering  
- Manual labeling of clustered identities  
- FastAI classifier training and saving  
- Gradio-based single and multi-face classification apps  
- Notebook-driven experimentation and visualization  

🎯 *Goal:* Demonstrate how modular design and minimal supervision can be used to build a scalable facial recognition system — from raw image data to real-time deployment.

---
## ✨ Key Features

- **Unsupervised Face Clustering**  
  Generate face embeddings and group similar faces without labels using clustering algorithms.

- **FastAI-Based Classifier Training**  
  Train a deep learning model on labeled face crops to recognize individual identities.

- **Multi-Face Detection & Classification**  
  Detect and classify multiple faces in a single image using bounding boxes and predictions.

- **Gradio-Powered Interactive Apps**  
  Launch real-time web apps for both single-face and multi-face classification.

- **Modular Notebook Design**  
  Each phase is isolated in its own Jupyter notebook for clarity, debugging, and experimentation.

- **Scalable & Reproducible Workflow**  
  Designed for easy extension, retraining, or deployment with minimal code changes.

---
## 🧱 Pipeline Phases

This project is structured into four distinct phases, each handled in its own notebook for clarity and modularity:

| Phase | Description |
|-------|-------------|
| **1. Data Preparation & Clustering** | Crop faces from raw images, generate embeddings, and cluster similar faces using unsupervised techniques. |
| **2. Classifier Training** | Manually label clustered identities and train a FastAI-based classifier to recognize individuals. |
| **3. Single-Face Classification App** | Build a Gradio app that detects and classifies a single face from an uploaded image. |
| **4. Multi-Face Classification App** | Extend the app to detect and classify multiple faces in group images using bounding boxes and predictions. |

---

## ⚙ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Daddy-Myth/FaceId-Pipeline-Clustering-to-MultiFace-Classification.git
cd FaceId-Pipeline-Clustering-to-MultiFace-Classification
```

### 2. Set Up the Environment

Using Conda (recommended):

```bash
conda env create -f environment.yml
conda activate faceid-pipeline
```

Or using pip:

```bash
pip install -r requirements.txt
```

### 3. Launch the Notebooks

Open Jupyter and run the notebooks in the `notebooks/` folder sequentially:

```bash
jupyter notebook
```

> 💡 Make sure to place your image dataset inside the `Images/` folder before running the notebooks.

---
