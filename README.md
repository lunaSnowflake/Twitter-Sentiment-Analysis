# Twitter-Sentiment-Analysis

Will use 2 main approaches to the sentimental analysis
- VADER (Valence Aware Dictionary sEntiment Reasoner) - Bag of words approach
- ROBERTA (Transformer) by Hugging Face🤗

- We will also run some prebuild Roberta pipelines.

## VADER Sentiment scoring

We'll use NLTK's `SentimentIntensityAnalyzer` to get the positive/negative/neutral scores of a text

- Uses Bag of words:
    - Stop words are removed
    - Each word is stored and combined for a final score
    
Remember it will score each word individually and then combines the scoring to check wheather the statement is positive or otherwise. Becuase of independent scoring, it does not take into account the relationship between words (context)


## Roberta - Pretrained Model

- Roberta is a Transformer
- Trained on Large corpus of data
- Transformer models not only account for words, but also for the context of a statement


## Conclusion:
As Roberta accounts for context, it is much more powerful than simple models like VADER which uses Bag of wrods approach.
