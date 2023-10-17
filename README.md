# Movie-Reviews-Sentiment-Analysis-using-PySpark
This repository contains code for performing sentiment analysis on movie reviews using PySpark. The analysis is done by counting the occurrences of positive and negative words in the reviews and assigning sentiments based on the counts.

## Prerequisites

Before running the code, ensure you have the following installed:

- Java 8: `sudo apt-get install openjdk-8-jdk-headless`
- Apache Spark 3.2.0: Download from [here](https://archive.apache.org/dist/spark/spark-3.2.0/spark-3.2.0-bin-hadoop3.2.tgz) and extract it.
- Python packages: `findspark`

## Setup

1. Install Java 8 and extract Apache Spark 3.2.0.
2. Install required Python packages: `pip install findspark`.
3. Clone this repository: `git clone <repository-url>`.
4. Place your movie review data in the specified directory: `/content/drive/MyDrive/Analysis/data_moviereviews`.
5. Update positive words in `pos.txt` and negative words in `neg.txt`.

## Usage

1. Open the Jupyter Notebook or Python environment where you have Spark set up.
2. Run the provided Jupyter Notebook or execute the Python script in your environment.

## File Descriptions

- `data_moviereviews`: Directory containing movie review files.
- `pos.txt`: File containing positive words.
- `neg.txt`: File containing negative words.
- `Sentiment_Analysis.ipynb`: Jupyter Notebook containing the code for sentiment analysis.

## Output

The analysis will generate a data frame containing the following columns:

- `filename`: Name of the movie review file.
- `positive_count`: Count of positive words in the review.
- `negative_count`: Count of negative words in the review.
- `sentiment`: Assigned sentiment based on word counts (either 'positive' or 'negative').
