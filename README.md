Sentiment Analysis and Visualization with VADER
This Python program performs sentiment analysis on a set of text data using the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool. The program analyzes the sentiment of each text entry, classifies it into positive, neutral, or negative categories, and visualizes the results.

Features
Sentiment Analysis:

Uses the VADER sentiment analysis tool to calculate sentiment scores for each text entry.
Classifies the sentiment as Positive, Neutral, or Negative based on the compound sentiment score.
Data Visualization:

Visualizes the distribution of sentiment categories (Positive, Neutral, Negative) using a bar chart.
Plots the distribution of sentiment scores using a histogram with a KDE (Kernel Density Estimate) plot.
Dependencies
To run this program, you'll need the following Python libraries:

pandas
matplotlib
seaborn
nltk
You can install these dependencies using pip:

pip install pandas matplotlib seaborn nltk

Additionally, you'll need to download the VADER lexicon using NLTK:

python -m nltk.downloader vader_lexicon

Usage
Set Up the Environment: Ensure you have Python installed along with the required libraries.

Run the Script: Execute the script to perform sentiment analysis on the text data and visualize the results.

python sentiment_analysis.py

View the Output: The program will display:
A bar chart showing the count of each sentiment category (Positive, Neutral, Negative).
A histogram showing the distribution of sentiment scores across all text entries.
How It Works
Data Input:

The program uses a small sample dataset containing ten text entries. These entries represent different opinions and statements.
Sentiment Analysis:

The program initializes the VADER sentiment analyzer and calculates a compound sentiment score for each text entry.
The sentiment score ranges from -1 (most negative) to 1 (most positive).
Sentiment Classification:

Based on the compound sentiment score:
Sentiment is classified as Positive if the score is ≥ 0.05.
Sentiment is classified as Negative if the score is ≤ -0.05.
Sentiment is classified as Neutral if the score is between -0.05 and 0.05.
Data Visualization:

The program visualizes the sentiment distribution using a bar chart, showing the number of Positive, Neutral, and Negative entries.
It also visualizes the distribution of sentiment scores using a histogram with a KDE plot, providing a more detailed view of sentiment score distribution.
Customization
Text Data: You can modify the data dictionary to analyze a different set of text entries.
Visualization Style: You can change the visualization styles (colors, sizes, etc.) by adjusting the parameters in the seaborn and matplotlib functions.
Example Output
Sentiment Distribution
A bar chart displaying the counts of Positive, Neutral, and Negative sentiments.
Sentiment Scores Distribution
A histogram with a KDE plot showing the distribution of sentiment scores across the text entries.

Author
This script was created as a demonstration of basic sentiment analysis using the VADER tool in Python.

