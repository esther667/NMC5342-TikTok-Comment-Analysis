# NMC5342 — TikTok Finance Comment Analysis

NMC5342 individual assignment analysing TikTok finance comments through text preprocessing, keyword analysis, TextBlob sentiment, Gensim LDA topics, and promotion sensitivity checks.

The project examines comments on **@dr.jubairsfinance** using the public TikTok sample from [Bright Data / luminati-io](https://github.com/luminati-io/Social-media-dataset-samples). Each observation is one comment.

## Notebook

[**NMC5342_A0352776R.ipynb**](NMC5342_A0352776R.ipynb) contains the annotated code, saved results and interpretations.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/esther667/NMC5342-TikTok-Comment-Analysis/blob/main/NMC5342_A0352776R.ipynb)

## Research questions

1. What topics do users discuss in this finance creator's comment section?
2. What sentiment does the comment text express?
3. How do sentiment and topic estimates change when suspected investment promotions are excluded?

## Workflow

- **Part 1:** Python loops, conditionals, word counts, and hashtag/mention extraction.
- **Part 2:** Data inspection, missing and duplicate checks, dates, and active users.
- **Part 3:** NLTK preprocessing, word frequencies, word clouds, and TF–IDF.
- **Part 4:** TextBlob polarity and subjectivity, Gensim LDA with 3–5 topics, visual comparisons, sensitivity checks, and brief reflection.
- **Part 5:** Interpretation and limitations.

The sample contains 1,000 comments. The selected account contributes 799 comments, of which 678 pass the English-language filter. The baseline promotion rule flags 63 of those comments. The LDA analysis uses 592 non-empty documents after its additional text filters.

## Run the analysis

1. Open the notebook using the Colab button above.
2. Choose **Runtime → Run all**.
3. The notebook installs its additional packages and downloads the NLTK resources.
4. Results are saved in `/content/nmc5342_outputs` in Colab.

The analysis uses pandas, NumPy, NLTK, scikit-learn, TextBlob, Gensim, Matplotlib, seaborn, langdetect, and wordcloud. The random seed is 42. Rerunning requires internet access. Changes to the upstream dataset or package versions may change the results.

## Interpretation and limits

The data are a convenience sample. They do not represent all comments on the account or all TikTok users. Sentiment scores describe lexical tone. Promotion flags identify suspected promotional wording and do not prove fraud. LDA themes overlap and remain exploratory.

The notebook includes saved outputs. This GitHub upload preserves those outputs; it does not document a new full execution. The separate 1,000–1,500-word assignment report is not included in this repository.

