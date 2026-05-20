# NeuroAssist — ML-Driven MRI Vision for Brain Tumor Analysis

A modular medical AI framework combining 2.5D U-Net brain tumor segmentation, volumetric quantification in mm³, and regression-based survival estimation. Deployed via a REST-based Flask backend. Published as a conference paper at the American University of Dubai.

## Why no code?

The full project includes a trained 2.5D U-Net model, the complete BraTS dataset, and all preprocessing pipelines. The total size exceeds 80GB which makes it impossible to host on GitHub. The conference paper included in this repository covers the full system architecture, methodology, results and deployment design in detail.

## What's in the paper

- 2.5D U-Net segmentation architecture across four MRI modalities (T1, T1ce, T2, FLAIR)
- Intelligent chunking into 256×256×12 input tensors preserving inter-slice context
- Volumetric reconstruction pipeline computing tumor volumes in mm³
- Regression-based survival estimation using cross-validated feature vectors
- REST-based Flask deployment backend with structured JSON outputs
- Peak validation Dice Similarity Coefficient: 0.7559
- Mean Intersection over Union: 0.6457
- Class-wise Dice: 0.7617 (edema), 0.7743 (enhancing), 0.6109 (necrotic core)

## Tech Stack

Python | TensorFlow/Keras | Flask | NiBabel | NumPy | BraTS Dataset | REST API | GPU Inference

## Team

Developed by Seya Makin, Toufic Al Akl, Mohannad Abou Rehab, Lina Noman and Harihar Rengan under the supervision of Dr. Vinod Pangracious, School of Engineering, American University of Dubai.
