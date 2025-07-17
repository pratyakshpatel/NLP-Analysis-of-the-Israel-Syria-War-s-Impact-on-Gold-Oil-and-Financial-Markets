# NLP-Analysis-of-the-Israel-Syria-War-s-Impact-on-Gold-Oil-and-Financial-Markets
Certainly, here is a README file for your project based on the provided codebook:

# Geopolitical Impact on Financial Markets: Topic Modeling Analysis

This project analyzes the impact of geopolitical events, specifically the Israel-Palestine conflict, on financial markets. It uses Latent Dirichlet Allocation (LDA) to identify key topics from a corpus of news articles and reports. By examining these topics, the project aims to understand the various narratives and their prevalence in financial and geopolitical discourse.

-----

## 📜 Table of Contents

  - [Project Overview](https://www.google.com/search?q=%23-project-overview)
  - [Methodology](https://www.google.com/search?q=%23-methodology)
  - [Key Findings](https://www.google.com/search?q=%23-key-findings)
  - [How to Use](https://www.google.com/search?q=%23-how-to-use)
  - [Dependencies](https://www.google.com/search?q=%23-dependencies)

-----

## 📝 Project Overview

This project explores the intricate relationship between geopolitical tensions and financial market stability. By leveraging Natural Language Processing (NLP) and topic modeling, it uncovers the underlying themes in news articles related to the Israel-Palestine conflict. The analysis provides insights into how different facets of the conflict are reported and their potential implications for the global economy.

-----

## 🛠 Methodology

The project follows a structured approach to analyze the text data:

1.  **Text Preprocessing**: The initial step involves cleaning the text data to make it suitable for analysis. This includes:

      * Removing non-alphabetic characters and digits.
      * Converting text to lowercase.
      * Eliminating common English stopwords.
      * Lemmatizing words to their base forms.
      * Filtering out a custom list of additional irrelevant words.

2.  **Bag-of-Words (BoW) Representation**: The cleaned text is transformed into a Bag-of-Words model, which represents each document as a collection of its word counts. This is a crucial step for preparing the data for the LDA model.

3.  **LDA Topic Modeling**: Latent Dirichlet Allocation (LDA) is employed to discover abstract topics within the text corpus. The model assumes that each document is a mixture of various topics and that each topic is characterized by a distribution of words.

4.  **Model Evaluation**: To determine the optimal number of topics, two key metrics are used:

      * **Coherence Score**: This measures the semantic similarity of words within a topic. A higher coherence score indicates more interpretable and meaningful topics.
      * **Mean Overlap**: This metric assesses the distinctiveness of topics by calculating the average proportion of shared words between them. A lower mean overlap is desirable for well-separated topics.

-----

## 📈 Key Findings

Based on the analysis of coherence scores and mean topic overlap, the model with **13 topics** was identified as the most suitable for this dataset. This model offers a high coherence score while maintaining a low mean overlap, indicating that the topics are both meaningful and distinct.

The 13 identified topics are:

| Topic ID | Top 10 Keywords |
| :--- | :--- |
| **Topic 1** | risk, africa, i, african, country, global, geopolitical, economy, report, political |
| **Topic 2** | jazeera, price, show, iranian, involvement, oil, rothman, keep, navigation, president |
| **Topic 3** | cent, investor, bond, cost, billion, rating, credit, last, due, concern |
| **Topic 4** | oil, energy, global, price, risk, economy, gas, center, business, new |
| **Topic 5** | credit, loan, card, business, personal, select, cnbc, small, investing, mortgage |
| **Topic 6** | oil, global, price, economy, energy, impact, cent, demand, wolf, real |
| **Topic 7** | price, share, stock, trading, bank, time, prime, result, offer, oil |
| **Topic 8** | price, share, bank, option, trading, chain, ipo, banking, future, stock |
| **Topic 9** | global, vantage, economy, oil, advertisement, recession, lead, firstpost, sport, major |
| **Topic 10** | cent, demand, comment, get, sale, activity, yearonyear, insight, auto, app |
| **Topic 11** | price, share, gold, loan, rate, bank, personal, stock, ipl, ipo |
| **Topic 12** | global, risk, geopolitical, energy, rating, supply, insight, trade, chain, featured |
| **Topic 13** | price, share, company, stock, bank, loan, oil, business, adani, tc |

-----

## 🚀 How to Use

To replicate this analysis, follow these steps:

1.  **Set up the environment**: Ensure you have Python 3 and the required dependencies installed.
2.  **Prepare the data**: Place your text files (`.txt`) in the specified directory.
3.  **Run the notebook**: Execute the cells in the `code.ipynb` notebook sequentially.

The notebook will automatically process the text data, build the LDA model, and save the identified topics and their frequencies to `LDA_Topics.xlsx` and `Topic_Frequencies_Model_13.xlsx` respectively.

-----

## 📦 Dependencies

This project relies on the following Python libraries:

  * `os`
  * `re`
  * `nltk`
  * `gensim`
  * `numpy`
  * `matplotlib`
  * `pandas`
  * `yfinance`

You can install the necessary packages using `pip`:

```bash
pip install nltk gensim numpy matplotlib pandas yfinance
```
