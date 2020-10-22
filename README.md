# DSCS-Dataset

In this repository we provide a new benchmark dataset Domain-Specific Complex Sentences dataset with human annotated semantic similarity values. 
We also provide the performance of word2vec, GloVe, BERT, RoBERTa and ALBERT word embeddings implemented using Sentence-BERT framework on the benchmark dataset.
|                      |                                              | Pearson's   Correlation |             |       | Spearman's   Correlation |             |       |
|----------------------|----------------------------------------------|-------------------------|-------------|-------|--------------------------|-------------|-------|
|                      |                                              | STS - test              | SICK - Test | DSCS  | STS - test               | SICK - Test | DSCS  |
| Unsupervised         | word2vec                                     | 62.61                   | 72.67       | 48.30 | 58.71                    | 62.13       | 49.04 |
|                      | Glove                                        | 45.42                   | 63.53       | 43.90 | 46.88                    | 55.59       | 50.14 |
|                      | word2vec + CS Corpus                         | 56.77                   | 67.75       | 52.35 | 53.27                    | 59.38       | 46.79 |
|                      | Glove + CS Corpus                            | 41.09                   | 60.44       | 48.02 | 42.85                    | 54.20       | 42.52 |
| Partially supervised | BERT large + NLI +   Mean Pooling            | 76.17                   | 73.65       | 54.78 | 79.19                    | 73.72       | 54.47 |
|                      | BERT base + NLI + Mean Pooling               | 74.11                   | 72.95       | 50.91 | 76.97                    | 72.89       | 47.73 |
|                      | RoBERTa large + NLI + Mean Pooling           | 76.26                   | 74.35       | 54.54 | 78.69                    | 74.01       | 46.36 |
|                      | RoBERTa base + NLI + Mean Pooling            | 74.58                   | 76.05       | 37.74 | 77.09                    | 74.44       | 39.48 |
|                      | ALBERT xxlarge + NLI + Mean Pooling          | 78.56                   | 77.78       | 45.44 | 79.55                    | 75.37       | 41.33 |
|                      | ALBERT xlarge + NLI + Mean Pooling           | 77.68                   | 73.90       | 54.90 | 80.12                    | 74.78       | 57.68 |
| Supervised           | BERT large + NLI +   STSB+ Mean Pooling      | 84.63                   | 80.97       | 71.11 | 85.25                    | 78.48       | 66.78 |
|                      | BERT base + NLI   +  STSB+ Mean Pooling      | 84.18                   | 82.16       | 67.79 | 85.04                    | 78.43       | 64.02 |
|                      | RoBERTa large + NLI   +  STSB+ Mean Pooling  | 85.54                   | 82.32       | 64.69 | 86.42                    | 78.40       | 60.48 |
|                      | RoBERTa base + NLI   +  STSB+ Mean Pooling   | 84.26                   | 81.78       | 50.57 | 85.26                    | 77.43       | 46.46 |
|                      | ALBERT xxlarge + NLI   + STSB + Mean Pooling | 92.58                   | 85.33       | 73.67 | 90.22                    | 80.03       | 67.54 |
|                      | ALBERT xlarge + NLI +   STSB + Mean Pooling  | 91.59                   | 83.28       | 71.45 | 90.73                    | 81.52       | 66.97 |
