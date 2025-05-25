# EndSARS Tweet Sentiment Analysis

This project performs a sentiment analysis on tweets about the **#EndSARS** movement, a significant social uprising in Nigeria. The movement saw Nigerian youths protesting against the Special Anti-Robbery Squad (SARS), a controversial unit of the Nigerian Police Force, accused of brutality, extortion, and targeting young people under the guise of combating cybercrime.

This analysis aims to uncover the prevailing sentiments expressed in tweets during the EndSARS protests, providing insights into public opinion and emotional tones surrounding the movement.


---

## Key Features

* **Tweet Collection (Implicit):** Assumes a dataset of EndSARS-related tweets is available or can be collected.

* **Sentiment Classification:** Categorizes tweets into positive, negative, or neutral sentiments.

* **Sentiment Score Visualization:** Plots the distribution of sentiment scores to show the overall emotional landscape.

* **Word Cloud Generation:** Creates a visual representation of the most frequently used words in the tweets, highlighting key themes and topics.

---

## Analysis & Visualization

The analysis was performed using **Python** and the following key libraries:

* `pandas`: For efficient data loading, manipulation, and cleaning of tweet data.

* `numpy`: For numerical operations.

* `matplotlib.pyplot`: For creating static visualizations, particularly the sentiment score plot.

* `seaborn`: For enhancing the aesthetics and statistical graphics of plots.

* `nltk` (Natural Language Toolkit): For text preprocessing tasks such as tokenization, stop word removal, and stemming/lemmatization.

* `TextBlob`: A simplified API for common natural language processing (NLP) tasks, used here for sentiment analysis.

* `wordcloud`: For generating the word cloud visualization.

The project generates:

1.  **Sentiment Score Plot:** A visual representation (e.g., histogram or density plot) showing the distribution of sentiment scores (polarity) across all analyzed tweets. This helps understand the overall emotional leaning of the discussion.

2.  **Word Cloud:** A graphical depiction of the most frequent words used in the tweets, with larger words indicating higher frequency. This provides a quick overview of the prominent themes and keywords associated with the EndSARS movement.

---

## Getting Started

To set up and run this sentiment analysis project locally, please follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone [Your GitHub Repository Link]
    cd [Your Repository Folder Name]
    ```

2.  **Install the required Python libraries:**
    It's highly recommended to use a virtual environment to manage dependencies.

    ```bash
    # Create a virtual environment
    python -m venv venv

    # Activate the virtual environment
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate

    # Install the libraries
    pip install pandas numpy matplotlib seaborn nltk textblob wordcloud
    ```

    *Note: After installing `nltk`, you might need to download specific NLTK data (e.g., stop words). This can typically be done within your Python script or interactively:*

    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

3.  **Prepare your data:**
    Ensure your tweet data (e.g., a CSV file named `endsars_tweets.csv`) is placed in the project directory. The script expects a column containing the tweet text.

4.  **Run the analysis:**
    Execute the main Python script that performs the sentiment analysis and generates the visualizations.

    ```bash
    python sentiment-analysis-on-endsars-tweets.ipynb
    ```

