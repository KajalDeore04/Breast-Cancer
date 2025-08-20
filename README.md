# Breast Cancer Detector

A web application that uses a machine learning model to predict whether breast cancer is malignant or benign based on medical features with 97% accuracy.  
**Live Demo:** [https://breast-cancer-xv3i.onrender.com/](https://breast-cancer-xv3i.onrender.com/)

---

## Features

- Upload or enter medical feature vectors to get predictions.
- "Load Sample Dataset" button to auto-fill example data.
- Modern, responsive UI with animated feedback.
- Powered by a trained Logistic Regression model (scikit-learn).

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/breast-cancer-detector.git
cd breast-cancer-detector
```

### 2. Install dependencies

Make sure you have Python 3.8+ installed.

```bash
pip install -r requirements.txt
```

### 3. Prepare the model

If you want to retrain the model:

- Edit and run `model.ipynb` to train and export `model.pkl`.
- Or use the provided `model.pkl`.

### 4. Run the app locally

```bash
python app.py
```

Visit [http://localhost:5000](http://localhost:5000) in your browser.

---

## Deployment

This app is deployed on [Render](https://render.com/).

To deploy yourself:

1. Push your code to a public GitHub repository.
2. Create a new **Web Service** on Render.
3. Set the build and start commands:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `python app.py`
4. Make sure `model.pkl` is included in your repo.

---

## Usage

- Click **Load Sample Dataset** to auto-fill a sample.
- Paste or enter a comma-separated feature vector (31 values).
- Click **Initialize Analysis** to get a prediction.

---

## File Structure

```
├── app.py                # Flask backend
├── model.ipynb           # Model training notebook
├── model.pkl             # Trained ML model
├── requirements.txt      # Python dependencies
├── breast cancer.csv     # Dataset
└── templates/
    └── index.html        # Frontend UI
```

---

## Tech Stack

- Python, Flask
- scikit-learn, pandas, numpy
- HTML, CSS (Bootstrap), JavaScript

---

## License

This project is for educational and research purposes only.  
Not for clinical use. Always consult medical professionals for diagnosis.

---

## Credits

- [UCI ML Breast Cancer Wisconsin (Diagnostic) Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
