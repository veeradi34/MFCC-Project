# MFCC-Based Song Clustering Project 🎵

This repository contains the code and methodology for clustering 115 unlabeled songs into six distinct categories using **Mel-Frequency Cepstral Coefficients (MFCCs)** and machine learning techniques. The project leverages audio feature extraction and unsupervised clustering to group songs into meaningful categories.

## 📂 Dataset

The dataset comprises 115 CSV files, each representing MFCC coefficients extracted from songs. Unfortunately, audio files are unavailable; the analysis is based solely on these coefficients. The categories targeted for clustering are:

1. **Indian National Anthem renditions**
2. **Marathi 'Bhav Geet'** sung by various artists
3. **Marathi Lavni songs**, predominantly sung by female artists
4. **Hindi film songs** sung by Asha Bhosale
5. **Hindi film songs** sung by Kishore Kumar
6. **English songs** by Michael Jackson

### Unique Dataset Features
- The **shortest song** in the dataset is always the **Indian National Anthem**.
- MFCC features provide a robust representation of audio characteristics.

## 🚀 Approach

### 1. Preprocessing
- **MFCC Extraction**: Extracted MFCC coefficients from the dataset for feature representation.
- **Normalization**: Standardized the features for better clustering performance.

### 2. Clustering
- **Clustering Algorithms**: Experimented with k-means and hierarchical clustering to identify 6 clusters.
- **Dimensionality Reduction**: Applied PCA to reduce feature dimensions while preserving significant variance.

### 3. Challenges
- Achieved good clustering results for **National Anthem**, **Kishore Kumar**, and **Michael Jackson** songs.
- Struggled with identifying **Asha Bhosale**, **Bhav Geet**, and **Lavni** categories accurately.
- **Imbalance in cluster sizes** and **overlap in audio features** posed challenges.

### 4. Observations
- Songs by **Asha Bhosale** had **low accuracy** due to overlap with other categories.
- **Shortest song heuristic** (National Anthem) was a key distinguishing feature.

## 📊 Results

| Category                  | Accuracy       |
|---------------------------|----------------|
| National Anthem           | High           |
| Kishore Kumar Songs       | High           |
| Michael Jackson Songs     | High           |
| Asha Bhosale Songs        | Low            |
| Marathi Bhav Geet         | Moderate       |
| Marathi Lavni Songs       | Moderate       |

## 🛠️ Technologies Used

- **Python** for coding
- **Pandas**, **NumPy** for data manipulation
- **Scikit-learn** for clustering and PCA
- **Matplotlib**, **Seaborn** for visualization



## 📝 Future Work

- Enhance feature engineering to better distinguish between overlapping categories.
- Incorporate deep learning models, such as **autoencoders**, for feature extraction.
- Experiment with advanced clustering techniques like **DBSCAN** or **Gaussian Mixture Models**.

## 💡 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
