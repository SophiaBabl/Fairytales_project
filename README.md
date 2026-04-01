# Once Upon a Dataset - Computational Analysis of Fairy Tale Originals, Adaptations, and AI-Generated Texts

A corpus-based study investigating thematic, emotional, and semantic shifts in fairy tales across three text types: original tales (Grimm & Andersen), contemporary adaptations (Wikipedia summaries), and AI-generated retellings (Microsoft Copilot).

---

## Project Overview

This project was developed as part of a seminar at the University of Regensburg and investigates whether and how fairy tales have changed from their 19th-century originals to contemporary adaptations. The analysis covers three parallel lines of inquiry:

- **Sentiment & Emotion Detection**: affective shifts across text types and author traditions
- **Topic Modelling**: thematic changes from original to adaptation
- **Word2Vec**: semantic shifts in vocabulary and meaning

The corpus draws on two canonical fairy tale traditions: the **Brothers Grimm** (folktale tradition) and **Hans Christian Andersen** (literary fairy tale tradition).

---

## Repository Structure

```
fairytale-corpus/
│
├── corpus/
│   ├── Metadata_Fairytale_Corpus.csv       # Metadata sheet of full corpus (Original, Wikipedia, Copilot)
│   ├── fairy_tale_corpus_complete.csv      # Full Corpus (Grimm - Original, Wikipedia, Copilot + Andersen - Original, Wikipedia, Copilot)
│   ├── fairytale_corpus_andersen.csv       # Full Andersen corpus (Original, Wikipedia, Copilot)
│   └── fairytale_corpus_grimm.csv          # Full Grimm corpus (Original, Wikipedia, Copilot)
│
├── notebooks/
│   ├── Corpus_EDA.ipynb                            # Exploratory data analysis & descriptive statistics
│   ├── Grimm_Fairytales_Sentiment_Emotion.ipynb    # Sentiment & emotion analysis - Grimm
│   ├── Andersen_Fairytales_Sentiment_Emotion.ipynb # Sentiment & emotion analysis - Andersen
│   ├── Topic Modeling
│   └── Word2Vec
│
├── results/
│   ├── Sentiment Analysis and Emotion Detection  # csvs and figures
│   ├── Topic Modeling
│   ├── Word2Vec
│
└── README.md
```

---

## Corpus

The corpus consists of **309 texts** across three types and two author traditions:

| Author   | Original | Wikipedia | Copilot | Total |
|----------|----------|-----------|---------|-------|
| Grimm    | 40       | 87        | 87      | 214   |
| Andersen | 15       | 40        | 40      | 95    |
| **Total**| **55**   | **127**   | **127** | **309**|

**Text types:**
- **Original**: sourced from established digital editions (Grimm: ChildTaleA dataset; Andersen: andersenstories.com)
- **Wikipedia**: plot summaries of film adaptations, capped at 5 per original fairy tale, each with a minimum of 10 sentences
- **Copilot**: AI-generated fairy tales produced by Microsoft Copilot based on the Wikipedia summaries using a standardized prompt

Adaptations span from **1920 to 2025**, with a concentration from the 1970s onward.

---

## Requirements

```bash
pip install pandas matplotlib seaborn transformers nltk scikit-learn tqdm
```

Notebooks were developed in **Google Colab**. To run locally, adjust file paths accordingly (remove Google Drive mounts).

---

## Authors

- **Sophia Babl**: Sentiment Analysis & Emotion Detection
- **Emily Heinz**: Topic Modelling
- **Oscar Aquite-Pena**: Word2Vec

University of Regensburg, Faculty of Language, Literature and Cultural Studies, 2026

Presented at the **16. Studierendenkongress der Komparatistik**, Martin-Luther-Universität Halle-Wittenberg, May 2025.
