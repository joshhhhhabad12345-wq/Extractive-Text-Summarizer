# Extractive Text Summarizer

A Python-based command-line tool for summarizing lengthy texts using an extractive summarization approach based on the TextRank algorithm.

## Features
- Extracts the most important sentences from a given text file.
- Uses `nltk` for natural language processing (tokenization, stop words removal).
- Uses `networkx` to calculate sentence rankings via PageRank algorithm.
- Easily customizable summary length via command-line arguments.

## Requirements
Ensure you have Python 3 installed. Install the necessary dependencies with:

```bash
pip install -r requirements.txt
```

## Usage
Run the summarizer using Python by passing the path to the text file you wish to summarize.

```bash
python summarizer.py path/to/your/textfile.txt
```

### Options
You can change the number of sentences you want in your summary using the `--lines` flag (default is 3).

```bash
python summarizer.py path/to/your/textfile.txt --lines 5
```

## Testing
To run the test suite, ensure `pytest` is installed:

```bash
pip install pytest
pytest test_summarizer.py
```
