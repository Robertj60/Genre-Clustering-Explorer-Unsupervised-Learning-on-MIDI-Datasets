# Genre-Clustering-Explorer-Unsupervised-Learning-on-MIDI-Datasets

An unsupervised machine learning project that discovers musical genres from MIDI files using clustering techniques.

### Key Features
- **Feature Extraction**: Extracts 25+ musical features from MIDI files
- **Clustering Algorithms**: K-Means, Hierarchical, GMM, DBSCAN
- **Dimensionality Reduction**: PCA, t-SNE, UMAP visualizations
- **Evaluation Metrics**: Silhouette score, Davies-Bouldin index, Calinski-Harabasz score

## 📊 Extracted Features

### Melodic Features
- Interval statistics (mean, std, range)
- Melodic contour complexity
- Pitch range and distribution

### Rhythmic Features
- Note density
- Rhythmic variability
- Syncopation score
- Tempo and stability

### Harmonic Features
- Chord complexity
- Dissonance scores
- Key signatures

### Structural Features
- Polyphony levels
- Total duration
- Dynamic range

## 🚀 Quick Start
```bash
# 1. Install dependencies
pip install numpy pandas scikit-learn matplotlib seaborn

# 2. Setup project and generate sample data
python setup_project_simple.py

# 3. Run clustering analysis
python quick_start.py
```

## 📁 Project Structure
```
genre-clustering-explorer/
├── data/
│   ├── raw/           # Raw MIDI files (organized by genre)
│   └── processed/     # Extracted features CSV
├── src/
│   ├── midi_processor.py    # Feature extraction
│   ├── clustering.py         # Clustering algorithms
│   └── dimensionality.py     # PCA/t-SNE/UMAP
├── models/
│   └── saved_models/         # Trained models
├── notebooks/                # Jupyter notebooks
└── docs/                     # Documentation
```

## 🔬 Methodology

1. **Feature Extraction**: Parse MIDI files and extract musical features
2. **Preprocessing**: Standardize features using StandardScaler
3. **Optimal Clusters**: Use elbow method and silhouette analysis
4. **Clustering**: Apply multiple algorithms and compare results
5. **Visualization**: Project to 2D using PCA, t-SNE, and UMAP
6. **Evaluation**: Analyze cluster quality and interpretability

## 📈 Results

The clustering successfully identifies distinct musical patterns:
- **Classical**: Smooth melodic lines, structured rhythm
- **Jazz**: Complex harmonies, high syncopation
- **Rock**: Power chords, steady beat, limited range
- **Electronic**: Repetitive patterns, mechanical precision

## 🛠 Technologies

- **Python 3.8+**
- **scikit-learn**: Clustering and preprocessing
- **pandas**: Data manipulation
- **matplotlib/seaborn**: Static visualizations
- **UMAP**: Advanced dimensionality reduction

## 📝 Future Enhancements

- [ ] Add Streamlit interactive dashboard
- [ ] Implement deep learning features (autoencoders)
- [ ] Support for more audio formats
- [ ] Real-time genre prediction
- [ ] Hierarchical genre taxonomy

## 👤 Author

Created for data analytics portfolio demonstrations.
