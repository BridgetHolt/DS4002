# DS4002 Prototyping Project 1: Celebrity & Non-Celebrity Makeup Brand Review Sentiment Analysis

## Software and Platform
- **Programming Language**: Python 3
- **Development Environment**: Google Colab
- **Libraries and Packages Used**:
  - *pandas* - for data manipulation and cleaning
  - *VADER Sentiment Analysis* - to perform sentiment analysis on review text
  - *matplotlib* - to create data visualizations
  - *seaborn* - another visualization tool
  - *wordcloud* - to create word clouds of string/text data from reviews
  - *os* - operating system module
  - *numpy* - numerical computation
  - *sklearn* - includes machine learning tools, such as regression and vectorization
  - *scipy.stats* - statistical tests - includes Levene's and Mann-Whitney U
- **Tools**:
  - *Web Scraper Chrome Extension* - to extract and scrape review data from Sephora's website

## Map of Documentation

- **Data Folder**
  - **Uncleaned Individual Data**
    - csvs for each product scraped (18 total)
  - **Cleaned Individual Data**
    - cleaned csvs for each product scraped - output from Script 1 (18 total)
  - combined_clean_data.csv - cleaned csv containing all product data 
 
- **Scripts**
  - 1_CleaningData.ipynb - first script including data cleaning processes for each inididual product data
    - Output: Cleaned Individual Data
  - 2_Combination_VADER_Anaylsis.ipynb - script combined clean data and initial VADER anaylsis
    -Output: combined_clean_data.csv
  - 3_Variance_and_DistributionTest.ipynb - script running statistical tests (Levene's and Mann-Whitney U) to test variance and distribution of celebrity and non-celebrity compound sentiment scores
  - 4_EDA_Plots.ipynb - script to create visualizations to understand compound sentiment anaylsis scores distributions
    - Output: Distribution of Compound Sentiment Scores Bar Graph.png, Sentiment (Positive, Neutral, Negative) by Brand Type Bar Graph.png, Sentiment Distribution by Makeup Brand Violin Plot.png, Sentiment Distrubtion of Celebrity vs. Non-Celebrity Makeup Brands Violin Plot.png, Sentiment Polarization by Celebrity vs. Non-Celebrity Brands Boxplot.png
  - 5_WordCloud_Analysis.ipynb - script to visualize key words in negative/positive and celebrity/non-celebrity product reviews
  - 6_Logistic_Regression.ipynb - script for analysing logistic regression

- **Output**
  - Distribution of Compound Sentiment Scores Bar Graph.png
  - Sentiment (Positive, Neutral, Negative) by Brand Type Bar Graph.png
  - Sentiment Distribution by Makeup Brand Violin Plot.png
  - Sentiment Distrubtion of Celebrity vs. Non-Celebrity Makeup Brands Violin Plot.png
  -  Sentiment Polarization by Celebrity vs. Non-Celebrity Brands Boxplot.png
  - References.md - includes references for product data and intial research on topics + VADER package
    
## Instructions for Reproducing the Results
1. Clean data found in /DATA/Uncleaned Individual Data folder with script 1_CleaningData.ipynb (repeat for each uncleaned data csv)
2. Combine data and perform VADER sentiment anaylsis with 2_Combination_VADER_Anaylsis.ipynb
3. Compute statistical tests to determine if celebrity and non-celebrity sentiment scores are significantly varianced and distributed
4. Create explority data anaylsis with 4_EDA_Plots.ipynb to create visualizations of data distributions
5. Visualize key words with 5_WordCloud_Analysis.ipynb
6. Analyze data through logistical regression with 6_Logistic_Regression.ipynb
7. Make conclusions about data and compare finding against hypothesis
