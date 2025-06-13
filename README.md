# AI Dev Cardiosense
This is my work environment for this project. No other else

## Project Overview

CardioSense is an AI-driven project developed under the **LPDP Team in the AI Development Division**, focusing on the detection and classification of critical heart arrhythmias using advanced deep learning and machine learning techniques. The project is currently in **Phase 2**, with emphasis on refining model accuracy and optimizing data workflows.

This repository includes the core architecture, data pipelines, training sets, and model outputs for real-time and batch arrhythmia classification, backed by physiological ECG signal analysis.

---

## What is Arrhythmia?

**Arrhythmia** refers to any abnormality in the rhythm of the heartbeat—either too fast, too slow, or irregular. While some arrhythmias are benign, others can lead to life-threatening complications. Accurate and early detection is crucial for effective intervention.

The CardioSense system focuses on detecting the following arrhythmia classes from ECG signals:

---

## ✅ Arrhythmia Classes Detected

### 1. Normal (N)

Represents a healthy, regular heartbeat pattern. This is the baseline against which abnormal rhythms are detected.

*Insert Normal ECG image here*

---

### 2. Premature Atrial Contraction (PAC)

A specific type of atrial ectopic beat. The heartbeat comes earlier than normal and originates in the atria. PACs can be triggered by stress, caffeine, or fatigue and are commonly benign but notable when frequent.

*Insert PAC image here*

---

### 3. Premature Ventricular Contraction (PVC)

A type of ventricular ectopic beat where the lower chambers beat prematurely. PVCs are characterized by wide and bizarre QRS complexes on ECG. Frequent PVCs may indicate underlying heart disease.

*Insert PVC image here*

---

### 4. Atrial Fibrillation (AFIB)

An irregular and often rapid heartbeat caused by chaotic electrical signals in the atria. AFIB increases the risk of stroke and heart failure. The ECG typically shows no clear P waves and irregular R-R intervals.

*Insert AFIB image here*

---

### 5. Ventricular Fibrillation (VF)

A critical and life-threatening rhythm where the ventricles quiver ineffectively, failing to pump blood. Immediate defibrillation is required. ECG shows rapid, erratic electrical activity with no identifiable QRS complexes.

*Insert VF image here*

---

### 6. Ventricular Flutter (VFL)

A fast but more organized rhythm than VF. VFL can quickly deteriorate into VF and requires urgent treatment. On ECG, it appears as rapid, sine wave-like oscillations without discernible P or T waves.

*Insert VFL image here*

---

### 7. Ventricular Tachycardia (VT)

A fast heart rhythm originating from the ventricles. It can be sustained or nonsustained, with potential progression to VF. ECG shows wide QRS complexes at a high rate.

*Insert VT image here*

---

## Methodology

We employ a hybrid approach:

- **Deep Learning Models**:
  - CNN, LSTM, CNN-LSTM, and Transformer variants
- **Machine Learning Models**:
  - Ensemble-based models such as Random Forests, SVM, and Gradient Boosting

In addition, we integrate a **custom Java-based ECG signal processing tool**, inspired by Python's `neurokit2`, to extract physiological features before classification.

---

## Team and Collaboration

This project is developed in collaboration with:

- **AI Engineer**: Model development and experimentation
- **Backend Engineer**: Model integration into services
- **Feature Engineer**: Java-based physiological signal extraction

Together, we are building a scalable, reliable AI solution for cardiovascular health.

---

## Folder Structure and Key Paths

### AF Database (Atrial Fibrillation and Related)

- `CardioSense\data\af-database`
- Current work folder: `CardioSense\data\af-database\Latest`

Contains:
- `Model/`: Trained models for AFIB and related arrhythmias
- `Datas/`: Processed datasets
- `<Arrhythmia-Class>/`: ECG segments per class (AFIB, PAC, etc.)

### VFDB (Malignant Ventricular Ectopy Database)

- `CardioSense\data\vfdb-database`
- Current work folder: `CardioSense\data\vfdb-database\Latest`

Contains:
- `Model/`: Models for VF, VT, and VFL
- `Datas/`: Train/test data
- `<Arrhythmia-Class>/`: Segments per arrhythmia

---

## Visual Overview

- AI pipeline diagram
- Signal segmentation visualization
- ECG overlays with detection annotations

---

## Contribution

This repository is currently developed for internal R&D under LPDP.

---

## Disclaimer

This system is under research and **not certified for clinical use**. Any clinical deployment must follow medical validation and regulatory approval processes.
