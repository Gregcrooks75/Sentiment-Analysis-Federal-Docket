# Sentiment Analysis on a Federal Docket

## Overview

This project performs sentiment analysis on public comments submitted to a federal docket titled **"Endangered and Threatened Species: Critical Habitat Designations for Florida Manatee and Antillean Manatee."** It employs **Natural Language Processing (NLP)** techniques to extract, process, and analyze public feedback, aiming to derive insights into public sentiment and highlight key themes and trends.

By analyzing these comments, the project sheds light on public opinion regarding federal regulations, identifies common concerns, and visualizes geographical trends in sentiment.

---

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Objectives](#objectives)
- [Setup Instructions](#setup-instructions)
- [Workflow](#workflow)
  - [Step 1: Data Extraction](#step-1-data-extraction)
  - [Step 2: Data Preprocessing](#step-2-data-preprocessing)
  - [Step 3: Exploratory Data Analysis (EDA)](#step-3-exploratory-data-analysis-eda)
  - [Step 4: Sentiment Analysis](#step-4-sentiment-analysis)
  - [Step 5: Geographical Analysis](#step-5-geographical-analysis)
- [Results](#results)
- [Actual Work Performed](#actual-work-performed)
- [Future Work](#future-work)
- [Contributions](#contributions)
- [License](#license)

---

## Project Structure

- **`Sentiment Analysis on a Federal Docket.ipynb`**:
  - Jupyter Notebook containing all analysis steps, including data extraction, preprocessing, EDA, and sentiment analysis.
- **`comments_downloader.py`**:
  - Python script for downloading comments from the federal docket via the Regulations.gov API.
- **`doc_comments.csv`**:
  - CSV file storing the extracted public comments for analysis.
- **`Document_Data/`**:
  - Directory containing metadata and text data for documents associated with the docket.
- **`Data_Augmentation_World_Cities.csv`**:
  - Supplementary dataset for mapping cities to geographical coordinates.
- **`README.md`**:
  - This document, providing an overview and instructions for the project.

---

## Objectives

1. **Data Extraction**: Gather public comments and metadata from the federal docket using the [Regulations.gov API](https://regulations.gov/).
2. **Sentiment Analysis**: Classify comments as positive, neutral, or negative to gauge public sentiment.
3. **Topic Discovery**: Identify key themes using n-grams and clustering techniques.
4. **Geographical Insights**: Map sentiment trends across cities or regions.
5. **Transparency**: Provide stakeholders with a detailed and reproducible analysis of public opinion.

---

## Setup Instructions

### Prerequisites

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Gregcrooks75/Sentiment-Analysis-Federal-Docket.git
