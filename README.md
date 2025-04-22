# Sentiment Analysis Machine Learning Project

## Overview
This project demonstrates a complete machine learning workflow for text sentiment analysis. The model classifies product reviews as positive or negative based on the review text.

## Features
- Text preprocessing pipeline including stopword removal and lemmatization
- TF-IDF vectorization for feature extraction
- RandomForest classifier for sentiment prediction
- Model evaluation with accuracy metrics, ROC curve, and confusion matrix
- Feature importance analysis

## Project Structure
```
sentiment-analysis-project/
├── README.md
├── data/
│   ├── raw_data.csv
│   └── processed_data.csv
├── notebooks/
│   └── sentiment_analysis.ipynb
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── model_training.py
│   └── model_evaluation.py
├── models/
│   └── sentiment_classifier.pkl
├── requirements.txt
└── presentation/
    └── sentiment_analysis_presentation.pptx
```

## Requirements
- Python 3.8+
- pandas
- numpy
- scikit-learn
- nltk
- matplotlib
- seaborn
- joblib

Install all requirements using:
```bash
pip install -r requirements.txt
```

## Usage

### Data Preprocessing
```bash
cd src
python data_preprocessing.py
```

### Model Training
```bash
cd src
python model_training.py
```

### Model Evaluation
```bash
cd src
python model_evaluation.py
```

## Results
The model achieves approximately 85% accuracy on the test dataset. The confusion matrix and ROC curve visualizations are available in the presentation folder.

## Key Findings
- Most important features for sentiment classification are words like "excellent", "awful", "great", and "terrible"
- The model performs well at distinguishing clearly positive and negative reviews
- Reviews with mixed or neutral sentiment pose the greatest challenge for accurate classification

## Future Improvements
- Implement more advanced NLP techniques like word embeddings (Word2Vec, GloVe)
- Experiment with deep learning models (LSTM, BERT)
- Collect more diverse training data
- Add multi-class sentiment classification (e.g., very negative, negative, neutral, positive, very positive)

## License
MIT License
