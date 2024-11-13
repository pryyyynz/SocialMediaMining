

# Aspect-Based Sentiment Analysis on LGBTQ+ Tweets

## Project Overview

This project performs Aspect-Based Sentiment Analysis (ABSA) on LGBTQ+ related tweets to analyze public sentiment and identify key discussion themes. The study classifies tweets based on sentiment polarity (positive, negative, or neutral) and identifies prominent topics associated with the LGBTQ+ community. By employing sentiment analysis techniques, this project sheds light on prevailing attitudes toward LGBTQ+ topics on social media.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
  - [Data Collection and Preparation](#data-collection-and-preparation)
  - [Sentiment Classification](#sentiment-classification)
  - [Aspect Identification](#aspect-identification)
- [Results](#results)
- [Usage](#usage)
  - [Requirements](#requirements)
  - [Installation](#installation)
  - [Running the Code](#running-the-code)
- [Conclusion](#conclusion)
- [References](#references)

## Dataset
The dataset used in this analysis contains 32,456 tweets with LGBTQ-related hashtags and keywords, sourced from Kaggle. This dataset includes information such as tweet time, date, retweets, likes, and language. The tweets were scraped in August 2022, focusing on discussions surrounding the LGBTQ+ community on X (formerly Twitter).

## Methodology

### Data Collection and Preparation
- **Data Cleaning:** Used Beautiful Soup for text conversion to handle abbreviations and informal language, and applied regular expressions to remove special characters, URLs, and emojis.
- **Lemmatization and Stopwords Removal:** Employed SpaCy for lemmatization and used stopword filtering to retain relevant content for analysis.

### Sentiment Classification
- **Tool Used:** TextBlob was used to calculate sentiment polarity scores, with values ranging from -1 (negative) to +1 (positive). Neutral tweets were also identified.
- **Subjectivity Scores:** Incorporated subjectivity scores to differentiate between personal opinions and factual content, adding a layer of depth to the sentiment analysis.

### Aspect Identification
- **Word Tokenization:** Extracted key aspects from the text by tokenizing words and selecting prominent topics relevant to LGBTQ discussions.
- **Most Frequent Terms:** Key terms such as "lgbt," "community," "pride," "support," "anti," and "rights" were identified as frequent aspects in the discourse.

## Results
- **Sentiment Distribution:** The analysis revealed that:
  - 49.8% of the tweets were positive, showing support for LGBTQ+ rights and pride events.
  - 24.5% were negative, with themes of discrimination and prejudice.
  - 25.7% were neutral, consisting of factual statements and news.
- **Aspect Analysis:** Positive aspects were commonly associated with pride and support, while negative aspects were linked to discrimination and anti-LGBTQ+ sentiment. Neutral discussions typically focused on general information.

## Usage

### Requirements
- Python 3.x
- Libraries: TextBlob, BeautifulSoup, SpaCy, NLTK

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/pryyyynz/SocialMediaMining
   ```
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Code
1. Load the dataset and perform data cleaning.
2. Run sentiment classification and aspect identification as described in the methodology.
3. Visualize results using word clouds and sentiment distribution charts.

## Conclusion
This project contributes to understanding the sentiment and topics discussed around LGBTQ+ issues on social media, showing the positive role that platforms like X play in LGBTQ+ discourse. The results are valuable for advocacy groups, policymakers, and social platforms working to foster inclusive environments.

## References
- Dataset: [LGBT Tweets on Kaggle](https://www.kaggle.com/datasets/vencerlanz09/lgbt-tweets)
- Additional references and methodologies are included in the research paper.

