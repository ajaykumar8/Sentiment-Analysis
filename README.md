
```markdown
# Sentiment Analysis

## Overview

This project implements a sentiment analysis tool that processes text data, specifically movie reviews and tweets, to determine their sentiment scores. The tool utilizes a lexicon-based approach, leveraging a predefined sentiment lexicon to compute sentiment scores for input text.

## Features

- **Data Loading**: Loads IMDB movie reviews and live Twitter data for analysis.
- **Tokenization**: Tokenizes text by removing punctuation and stop words.
- **Sentiment Scoring**: Calculates sentiment scores based on a sentiment lexicon.
- **Data Visualization**: Analyzes sentiment across different tweets to summarize public opinion.

## Requirements

- Python 3.x
- Libraries:
  - `nltk`
  - `json`
  - `urllib`
  - `tkinter`

You can install the necessary libraries using pip:

```bash
pip install nltk
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/ajaykumar8/sentiment-analysis.git
   cd sentiment-analysis
   ```

2. Download the necessary NLTK data files:

   ```python
   import nltk
   nltk.download('stopwords')
   nltk.download('punkt')
   ```

3. Prepare the lexicon file (`lexicon.txt`) with sentiment scores. Ensure the format is correct as follows:

   ```
   word1   score1
   word2   score2
   ...
   ```

4. Prepare a JSON file containing tweets in the following format:

   ```json
   [
     {"text": "Tweet text 1"},
     {"text": "Tweet text 2"},
     ...
   ]
   ```

5. Run the script to perform sentiment analysis:

   ```python
   python sentiment_analysis.py
   ```

## Functions

### `tokenize(doc)`
- **Input**: A string of text (document).
- **Output**: A list of tokens (words) after removing punctuation and stop words.

### `sentiment_score(doc)`
- **Input**: A string of text (document).
- **Output**: A dictionary containing words and their corresponding sentiment scores from the lexicon.

### `score_message(doc)`
- **Input**: A string of text (message).
- **Output**: The overall sentiment score for the message.

## Contributing

Contributions are welcome! If you have suggestions for improvements or bug fixes, please create a pull request or open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [NLTK Documentation](https://www.nltk.org/)
- [Google Cloud Storage](https://cloud.google.com/storage)

```

