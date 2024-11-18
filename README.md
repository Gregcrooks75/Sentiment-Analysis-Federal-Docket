# Sentiment Analysis of Federal Docket

This project aims to perform sentiment analysis on public comments submitted to the Federal Docket, providing insights into public opinion on various federal regulations and notices.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Sentiment Analysis](#sentiment-analysis)
- [Results](#results)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Federal Docket Management System (FDMS) is a repository of federal regulations and related documents. Analyzing the sentiment of public comments can provide valuable insights into public opinion and the potential impact of regulations.

## Project Structure

The repository comprises the following files and directories:

- `Document_Data/`: Directory containing raw documents and data files related to the Federal Docket.
- `Data_Augmentation_World_Cities.csv`: CSV file used for data augmentation, possibly containing a list of world cities to enrich the dataset.
- `Sentiment Analysis on a Federal Docket.ipynb`: Jupyter Notebook detailing the step-by-step process of performing sentiment analysis on the collected data.
- `comments_downloader.py`: Python script designed to download public comments from the Federal Docket.
- `doc_comments.csv`: CSV file containing the extracted comments from the Federal Docket, serving as the primary dataset for analysis.

## Data Collection

Data was collected from the [Regulations.gov](https://www.regulations.gov/) website, which provides access to various federal documents and public comments. The `comments_downloader.py` script automates the process of fetching public comments related to specific dockets.

## Data Preprocessing

The collected data underwent the following preprocessing steps:

- **Cleaning**: Removal of HTML tags, special characters, and irrelevant information.
- **Tokenization**: Breaking down text into individual words or tokens.
- **Lemmatization**: Reducing words to their base or root form.
- **Stopword Removal**: Eliminating common words that do not contribute to sentiment (e.g., "and", "the", "is").

These steps are detailed in the `Sentiment Analysis on a Federal Docket.ipynb` notebook.

## Sentiment Analysis

Sentiment analysis was conducted using the following approaches:

- **Lexicon-Based Methods**: Utilizing predefined dictionaries to assign sentiment scores to words.
- **Machine Learning Models**: Training classifiers on labeled datasets to predict sentiment.
- **Deep Learning Models**: Implementing models like BERT for more nuanced sentiment detection.

The implementation details and code are provided in the Jupyter Notebook.

## Results

The analysis revealed the following insights:

- **Overall Sentiment**: Majority of the public comments exhibited a positive sentiment towards the proposed regulations.
- **Topic-Specific Sentiment**: Certain topics, such as environmental regulations, garnered more negative sentiments compared to others.
- **Temporal Trends**: Sentiment trends shifted over time, correlating with political and economic events.

Detailed results and visualizations are available in the notebook.

## Usage

To replicate the analysis:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Gregcrooks75/Sentiment-Analysis-Federal-Docket.git
