# Sentiment Analysis on Federal Docket Comments

This project conducts a comprehensive sentiment analysis of public comments submitted to the federal docket titled "Heat Injury and Illness Prevention in Outdoor and Indoor Work Settings." Utilizing advanced Natural Language Processing (NLP) techniques, the analysis aims to extract, process, and interpret public feedback, providing valuable insights into public sentiment and highlighting key themes and trends related to the proposed regulation.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Sentiment Analysis](#sentiment-analysis)
- [Geospatial Analysis](#geospatial-analysis)
- [Visualization](#visualization)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Occupational Safety and Health Administration (OSHA) has proposed a rule titled "Heat Injury and Illness Prevention in Outdoor and Indoor Work Settings." This proposal is documented under docket OSHA-2021-0009. Public comments on such proposals are crucial as they reflect the concerns, support, and suggestions of various stakeholders, including workers, employers, industry representatives, and the general public. Analyzing these comments provides a deeper understanding of public opinion, potential challenges, and areas of consensus or contention regarding the proposed regulation.

## Project Structure

The repository is organized as follows:

- `Document_Data/`: Contains raw documents and data files related to the federal docket. This directory includes the original public comments and associated metadata.
- `Data_Augmentation_World_Cities.csv`: A CSV file used for data augmentation, containing a comprehensive list of world cities along with their geographical coordinates. This dataset assists in mapping comment origins for geospatial analysis.
- `README.md`: The current file, providing an overview, detailed instructions, and insights into the project's objectives and methodologies.
- `Sentiment Analysis on a Federal Docket.ipynb`: A Jupyter Notebook that offers a step-by-step walkthrough of the sentiment analysis process, including data preprocessing, model implementation, and result interpretation.
- `comments_downloader.py`: A Python script designed to automate the downloading of public comments from the federal docket. This script ensures efficient and systematic data collection.
- `doc_comments.csv`: A CSV file containing the downloaded comments along with relevant metadata such as comment IDs, submission dates, and author information.
- `Sentiment_Analysis_Map.html`: An interactive HTML file visualizing the geospatial distribution of sentiments across different regions, providing a geographical perspective on public opinion.

## Data Collection

Data collection is a critical component of this project. The `comments_downloader.py` script is tailored to interface with the Federal Docket Management System (FDMS), specifically targeting docket OSHA-2021-0009. This script automates the retrieval of public comments, ensuring that the data is collected systematically and efficiently. Users should ensure they have the necessary permissions and adhere to any usage policies when accessing and utilizing this data. It's also advisable to review the terms of service and data usage policies of the FDMS to ensure compliance.

## Data Preprocessing

Effective data preprocessing is essential for accurate sentiment analysis. The preprocessing pipeline includes:

- **Text Cleaning**: This step involves removing special characters, numbers, punctuation, and other non-alphabetic elements that do not contribute to the sentiment analysis. It also includes converting all text to lowercase to maintain consistency.
- **Tokenization**: The cleaned text is split into individual words or tokens. Tokenization facilitates the analysis of word frequencies and patterns within the text.
- **Lemmatization/Stemming**: Words are reduced to their base or root form. For instance, words like "running," "ran," and "runs" are reduced to "run." This normalization process ensures that different forms of a word are analyzed as a single entity.
- **Stop Words Removal**: Common words that do not carry significant meaning (e.g., "and," "the," "is") are removed. Eliminating these stop words focuses the analysis on words that contribute more directly to the sentiment.

These preprocessing steps are implemented in the `Sentiment Analysis on a Federal Docket.ipynb` notebook, ensuring the text data is prepared appropriately for subsequent analysis.

## Sentiment Analysis

The core of this project is the sentiment analysis of public comments. The process involves:

- **Model Selection**: Choosing appropriate sentiment analysis models or libraries. This project explores various models, including traditional machine learning algorithms and advanced deep learning models, to determine the most effective approach for this dataset.
- **Implementation**: Applying the selected models to the preprocessed data. This includes training the models (if necessary), making predictions, and evaluating their performance.
- **Evaluation**: Assessing the performance and accuracy of the sentiment analysis models. Metrics such as accuracy, precision, recall, and F1-score are calculated to evaluate the models. Cross-validation techniques are also employed to ensure the robustness of the results.

The detailed implementation and evaluation processes are documented in the `Sentiment Analysis on a Federal Docket.ipynb` notebook.

## Geospatial Analysis

Understanding the geographical distribution of sentiments adds a valuable dimension to the analysis. This involves:

- **Data Augmentation**: Utilizing the `Data_Augmentation_World_Cities.csv` file to map city names mentioned in the comments to their corresponding geographical coordinates. This mapping enables the association of comments with specific locations.
- **Mapping**: Visualizing the sentiment distribution across different regions using geospatial plotting libraries. The `Sentiment_Analysis_Map.html` file provides an interactive map that displays the origin of comments and their associated sentiments, offering insights into regional variations in public opinion.

## Visualization

Visual representations are crucial for interpreting and communicating the results of the analysis. The project employs various visualization techniques:

- **Sentiment Distribution Charts**: Bar charts and pie charts illustrate the overall distribution of sentiments (e.g., positive, negative, neutral) across all comments.
- **Word Clouds**: Highlight the most frequently occurring words within each sentiment category, providing a visual representation of common themes and topics.
- **Geospatial Maps**: Interactive maps display the geographical distribution of sentiments, allowing users to explore regional patterns and trends.

These visualizations are integrated into the Jupyter Notebook and the `Sentiment_Analysis_Map.html` file, facilitating an intuitive understanding of the analysis results.

## Usage

To replicate or build upon this analysis:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Gregcrooks75/Sentiment-Analysis-Federal-Docket.git
