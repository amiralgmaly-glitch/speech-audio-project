# YESNO and VOiCES: Audio Classification and Voice Activity Detection

**Student:** Abdulameer Farhan Aljmmali  
**Student ID:** 404131110  
**Course:** Speech and Audio Processing

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/amiralgmaly-glitch/speech-audio-project/blob/main/YESNO_VOiCES_Python_Project_Abdulameer_Aljmmali.ipynb)

## Project files

| File | Description |
| --- | --- |
| [Report (PDF)](YESNO_VOiCES_Report_Abdulameer_Aljmmali.pdf) | Method, results and discussion for all three tasks |
| [Code (Jupyter Notebook)](YESNO_VOiCES_Python_Project_Abdulameer_Aljmmali.ipynb) | All experiments, with results and figures |

## Tasks

1. **YESNO:** classify each spoken word as "yes" or "no" with five classifiers (KNN, SVM, Decision Tree, Random Forest, Logistic Regression).
2. **VOiCES:** classify recordings by background distractor (none, babble, music, television).
3. **VAD:** detect speech frames with WebRTC VAD at four aggressiveness levels.

## Results

**YESNO (5-fold cross-validation, grouped by recording)**

| Method | Best classifier | Word accuracy | All 8 words correct |
| --- | --- | --- | --- |
| Whole-recording features (baseline) | Logistic Regression | 0.565 | 0.017 |
| **Word segmentation** | **Random Forest** | **0.963** | **0.883** |

**WebRTC VAD (60 YESNO recordings)**

| Aggressiveness | Precision | Recall | F1 |
| --- | --- | --- | --- |
| 0 | 0.706 | 0.993 | 0.825 |
| 1 | 0.708 | 0.990 | 0.826 |
| 2 | 0.804 | 0.978 | 0.882 |
| **3** | **0.867** | 0.957 | **0.910** |

## How to run

Open the notebook in Google Colab and choose **Runtime -> Run all**.
