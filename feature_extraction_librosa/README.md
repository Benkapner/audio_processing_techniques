# 🎵 Turning Songs into Tabular Data with Librosa

A practical project demonstrating how to transform unstructured audio files into structured, interpretable tabular data using Python’s `librosa` library.

## 📌 Overview

Working with audio for machine learning can sometimes feel like a black box, especially if you're more comfortable with tables than spectrograms. This project bridges that gap by walking through the complete pipeline of feature extraction from `.mp3` files and compiling those features into a pandas DataFrame, making the data ready for standard machine learning workflows.

## 📂 Contents

- `feature_extraction.ipynb`: Step-by-step tutorial for audio feature extraction using `librosa`.
- `classification_example.ipynb`: Demonstrates how to use the extracted features in a basic classification task.
- data folder are two free songs with no copyrights I have downloaded from https://pixabay.com/ 

## 🎧 Features Extracted

The project extracts interpretable features from audio, including:

- **Tempo and Beat Count**
- **Harmonic and Percussive Content**
- **RMS (Root Mean Square) Energy**
- **Dynamic Range**
- **Zero Crossing Rate (ZCR)**
- **Chroma Features**
- **MFCCs (Mel-Frequency Cepstral Coefficients)**
- **Spectral Features**:
  - Spectral Centroid
  - Spectral Bandwidth
  - Spectral Rolloff
  - Spectral Contrast
  - Spectral Flatness
- **Onset Strength**
- **Low, Mid, and High Frequency Energy Ratios**

Each feature is summarized using simple statistics (mean, std, min, max) and compiled into a tabular format.

## 🚀 Getting Started

### Installation

```bash
pip install librosa matplotlib pandas numpy
```

## ▶️ Run the Notebooks

- Start with **`feature_extraction.ipynb`** to extract features from `.mp3` files.
- Continue with **`classification_example.ipynb`** to apply machine learning models to the extracted features as an example use for the features extracted.

## 📊 Sample Output

A sample of the resulting tabular data:

| song             | tempo | beat_count | rms_average | chroma_mean | ... |
|------------------|-------|------------|-------------|-------------|-----|
| Rock             | 120.1 | 252        | 0.188       | 0.543       | ... |
| Classical Piano  | 86.1  | 75         | 0.072       | 0.491       | ... |

## 📚 References

- [Librosa Documentation](https://librosa.org/)
- McFee, B., et al. (2015). _librosa: Audio and music signal analysis in Python._  
  _Proceedings of the 14th Python in Science Conference._

