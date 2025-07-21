# Homonyms Problem in Text Analysis
1- Dataset : "https://www.kaggle.com/datasets/mohammedbahgat/homonym-sentiment-dataset"
2- Notebook : "https://www.kaggle.com/code/mohammedbahgat/homonyms-problem-in-the-text/notebook?scriptVersionId=251497179"

## Overview:
A deep learning project that addresses the contextual ambiguity challenge in sentiment analysis where identical words express different sentiments based on surrounding context. The system uses transformer-based models to distinguish between multiple meanings of homonym words.

## Problem Statement:
Traditional NLP methods fail when processing homonyms - words that have identical spelling but different meanings depending on context. For example:

### "I hate the selfishness in you" → Negative sentiment

### "I hate anyone who hurts you" → Positive sentiment

This project implements contextual understanding to resolve such ambiguities in sentiment classification.

## Features:
1- Context-aware sentiment analysis for homonym words

2- Multi-model comparison between traditional and transformer approaches

3- Custom dataset creation with 100 carefully annotated homonym examples

4- Real-time sentiment prediction with confidence scoring

## Model Architectures
1- DeBERTa-v3-base: Advanced transformer with disentangled attention

2- BERT-base-uncased: Standard transformer baseline

3- Traditional baselines: TF-IDF + Logistic Regression for comparison

## Custom Homonyms Sentiment Dataset
1- Size: 100 homonym word samples

2- Structure: 2 sentences per word (positive/negative pair)

3- Total: 200 sentences for training

4- Quality: Hand-crafted annotations ensuring clear sentiment contrast

5- Split: 80% training, 20% testing

## Performance Results
Model Comparison
Model	Accuracy	F1-Score	Status
DeBERTa-v3	84.85%	0.848	Excellent
TF-IDF + LR	48.78%	0.49	Baseline
BERT-base	48.48%	0.336	Failed

## Key Findings
1- DeBERTa-v3 breakthrough: Dramatic jump from 48% to 84.85% accuracy in final epoch

2- BERT failure: Standard BERT performed worse than traditional methods

3- Context importance: Advanced attention mechanisms crucial for homonym disambiguation

## Applications
1- Social media monitoring: Context-aware sentiment analysis

2- Customer feedback analysis: Accurate interpretation of ambiguous expressions

3- Content moderation: Improved understanding of contextual meaning

## Technologies
1- Core Stack: Python 3.10+, PyTorch, Transformers (Hugging Face)
2- Analysis Tools: Scikit-learn, Pandas, NumPy
3- Visualization: Matplotlib, Seaborn
4- Environment: Jupyter Notebook
