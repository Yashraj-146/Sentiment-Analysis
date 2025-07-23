# Sentiment Analysis Using Hugging Face Transformers

This repository demonstrates sentiment analysis using the Hugging Face Transformers library. The project leverages pre-trained models to classify text as positive or negative with high accuracy.

## Features

- Utilizes the `distilbert-base-uncased-finetuned-sst-2-english` model for sentiment classification.
- Includes a streamlined pipeline for sentiment analysis.
- Demonstrates user-friendly outputs with sentiment labels and confidence scores.

## Requirements

To run the code in this repository, you need to have the following dependencies installed:

- `transformers`
- TensorFlow-based utilities (`tf_keras`)
- Python 3.9 or later

Install the dependencies using pip:

```bash
pip install transformers
```

## Usage

The main notebook, `Sentiment_analysis_HF.ipynb`, showcases how to use the Hugging Face Transformers library for sentiment analysis.

### Example

The pipeline is initialized as follows:

```python
from transformers import pipeline

sentiment_analyzer = pipeline("sentiment-analysis", model="distilbert-base-uncased-finetuned-sst-2-english")
result = sentiment_analyzer("I love this!")
print(result)  # Output: [{'label': 'POSITIVE', 'score': 0.9998764991760254}]
```

You can analyze custom sentences by modifying the input text:

```python
sentiment_analyzer("Shane Watson is the best player in the world!")
```

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/Yashraj-146/Sentiment-Analysis.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Sentiment-Analysis
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Sentiment_analysis_HF.ipynb
   ```

4. Run the cells to execute the sentiment analysis pipeline.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to contribute, raise issues, or reach out for collaboration opportunities!
