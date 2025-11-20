
## Project: Spoken Language Processing Course Projects  
**Course:** Spoken Language Processing — Spring 2024/2025  
**Institution:** Birzeit University  

---

## 📁 Project 1: Speaker Identification Using MFCC Features and GMM/SVM Classifiers

### 📌 Overview
This project implements a speaker identification system using **Mel-Frequency Cepstral Coefficients (MFCCs)** with delta and delta-delta coefficients for feature extraction, and **Gaussian Mixture Models (GMMs)** and **Support Vector Machines (SVMs)** for classification.

### 👥 Authors
- Noor Shamali (1200016)  
- Dana Ghnimat (1200031)  
- Leyan Buirat (1211439)

### 🛠️ Methodology
1. **Data Preprocessing**: Audio files organized into train/test directories.
2. **Feature Extraction**: 45-dimensional MFCC features (15 static + 15 delta + 15 delta-delta) per frame, summarized to 90-dimensional vectors per file.
3. **Model Training**:
   - GMM per speaker
   - SVM with linear/RBF kernel
4. **Evaluation**: Accuracy, F1-score, recall, confusion matrices.

### 📊 Results
- **Best Model**: SVM with RBF kernel
- **Accuracy**: 72.4%
- **Macro F1-Score**: 0.715

### 📂 File Structure
```
/spokentests/
├── Train/
│   └── [speaker_id]/wav/*.wav
└── Test/
    └── [speaker_id]/*.wav
```

### 🚀 How to Run
1. Upload the dataset to Google Drive.
2. Open the Colab notebook.
3. Mount Google Drive and set paths.
4. Run data loading, feature extraction, training, and evaluation cells.

### 📈 Visualizations
- PCA plots of GMM components
- Histograms with Gaussian fits
- Confusion matrices

---

## 📁 Project 2: Arabic /r/ Sound Disorder Identification

### 📌 Overview
This project aims to classify the pronunciation disorder of the Arabic phoneme **/r/** when it appears at the beginning of a word. The disorder types are:

1. Distortion  
2. Deletion  
3. Substitution by /gh/  
4. Substitution by /l/  
5. Normal (correct) pronunciation

### 🎯 Goal
Build a model to classify the type of /r/ sound disorder using audio samples.

### 📂 Dataset
- **Train/Test splits** are provided in a shared Google Drive folder:  
  [Download Dataset](https://drive.google.com/drive/folders/13PPVmCAlbzGkzOvQxaB3NTcfUkG6GB?usp=sharing)

### 🛠️ Suggested Tools
- **SFS**, **Praat**, **Voicebox**, **Netlab**, **HTK**, **Kaldi**
- **Python environments**: Google Colab, Kaggle

### 📊 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score

### 📚 References
- [Wocci 2016 Paper](https://fada.birzeit.edu/bitstream/20.500.11889/4352/1/1-5_wocci2016.pdf)  
- [Additional Reference](https://drive.google.com/file/d/1ipKD9c29YaUpCPUJ0gMUzmntowdM9TDQ/view?usp=sharing)

---

## 🧩 General Requirements

### 📋 Report Format
- Use **IEEE conference template**
- 2–4 pages
- Include:
  - Title, authors, IDs
  - Abstract (< 200 words)
  - Introduction, Related Work, Methodology, Experiments, Results, Conclusion, References

### 🧪 Programming
- Python recommended (librosa, scikit-learn, matplotlib, etc.)
- MATLAB tools also acceptable (Voicebox, Netlab, etc.)

---

## 👨‍🔧 Team Participation (Project 1 Example)
- **Noor Shamali**: MFCC feature extraction + report  
- **Dana Ghnimat**: GMM/SVM training + evaluation  
- **Leyan Buirat**: Data organization + visualizations + report

---

## 📬 Submission
- Deadline: **Sunday, June 15, 2025**
- Submit via **ITC (Moodle)**

---

## 📎 Related Files
- `Speaker_Identification_Notebook.ipynb` (Colab notebook for Project 1)
- `Project_Report.pdf` (Final report in IEEE format)
- `Dataset/` (Local or Drive-based audio data)

---

