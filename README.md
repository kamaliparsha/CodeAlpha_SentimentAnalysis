# CodeAlpha Sentiment Analysis — Movie Reviews

## Project Overview

This project performs sentiment analysis on movie reviews using Python and the VADER sentiment analysis tool. It predicts whether a review expresses positive, negative, or neutral sentiment and evaluates predictions against the dataset's original labels.

## Internship

**CodeAlpha Data Analytics Internship — Task 4: Sentiment Analysis**

## Dataset

- **Source:** NLTK Movie Reviews corpus
- **Records:** Approximately 2,000 movie reviews
- **Original labels:** Positive (`pos`) and negative (`neg`)

The original labels represent the dataset's ground truth; they are separate from the sentiments predicted by VADER.

## Tools and Technologies

- Python
- Pandas and NumPy
- NLTK
- VADER Sentiment Analyzer
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

## Project Workflow

1. Load the movie reviews corpus.
2. Prepare the review text and original labels.
3. Initialize the VADER sentiment analyzer.
4. Predict sentiment using VADER compound scores.
5. Compare predictions with original labels.
6. Generate a sentiment distribution chart and confusion matrix.
7. Save prediction results and evaluation summaries.

## Results

- Reviews analyzed: **2,000**
- Positive predictions: **1,382**
- Negative predictions: **617**
- Neutral predictions: **1**
- Binary evaluation coverage: **1,999 reviews**
- Accuracy on non-neutral predictions: **63.53%**

The neutral prediction was excluded from the binary classification evaluation because the original dataset contains only positive and negative labels. Results reflect this dataset and the chosen VADER prediction method.

## Visualizations

- Distribution of predicted sentiment
- Confusion matrix comparing original and predicted sentiment

## Generated Outputs

The notebook creates an `outputs` folder containing:

- `sentiment_predictions.csv`
- `sentiment_distribution.png`
- `confusion_matrix.png`
- `confusion_matrix.csv`
- `classification_report.csv`
- `evaluation_summary.csv`

These files are generated when the notebook runs; they are not automatically uploaded to GitHub.

## How to Run

1. Open `CodeAlpha_SentimentAnalysis.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. Allow NLTK to download the required corpus and VADER lexicon when prompted.
4. Review the prediction results, evaluation metrics, and charts.

Install dependencies if needed:

```bash
pip install pandas numpy nltk matplotlib seaborn scikit-learn
```

## Limitations

VADER is a rule- and lexicon-based sentiment analyzer. It may misclassify movie reviews that contain sarcasm, complex context, or nuanced opinions. The measured accuracy is specific to this dataset and setup and should not be treated as a general benchmark for all sentiment-analysis tasks.

## Acknowledgements

The movie reviews corpus is provided through NLTK. VADER is used for sentiment scoring. This project was developed for educational purposes as part of the CodeAlpha Data Analytics Internship.
