# 🔍 Keyhole-Beta
PLEASE NOTE THIS APP IS STILL IN BETA. ISSUES ARE EXPECTED TO OCCUR. CORE FEATURES WORK WITH MINOR BUGS. 

**Keyhole-Beta** is a desktop tool that allows users to analyze website content for keyword frequency, readability, sentiment, and automatic summarization. Built with a focus on simplicity and user experience, Keyhole-Beta combines NLP, sentiment analysis, and modern GUI design to provide rich insights from web pages.

## 🚀 Features

- **Summarization**: Automatically condense full pages or sections using transformer-based models.
- **Sentiment Analysis**: Understand the tone of content with VADER sentiment scores.
- **Readability Metrics**: Includes Flesch Reading Ease scoring.
- **Keyword Extraction**: Displays the top 10 most frequent words, with optional exclusion filters.
- **Domain Crawling**: Recursively analyze multiple pages within a domain.
- **Configurable Presets**: Save and load excluded keyword sets.
- **Modern GUI**: Built with `customtkinter` for a sleek dark-themed interface.

## 🛠️ Installation

### Requirements

- Python 3.8+
- Dependencies listed in `requirements.txt`:
  - `transformers`
  - `vaderSentiment`
  - `beautifulsoup4`
  - `customtkinter`
  - `textstat`
  - `requests`

Install dependencies:

```bash
pip install -r requirements.txt
```

### Optional: GPU acceleration for transformers
To speed up summarization, configure your environment with CUDA support.

## 💡 Usage

### GUI Mode

Run the application using:

```bash
python main.py
```

You can:

- Enter a URL
- Choose analysis mode: `section`, `full`, or `domain`
- Set summary size: `small`, `medium`, `large`
- Optionally specify section titles or exclude keyword sets

Reports are saved to your OneDrive `Documents/Reports` directory by default.

### Report Output

Each report contains:
- Top 10 common words (excluding custom-defined stop words)
- Text summary
- Sentiment analysis
- Readability score

## 📁 Directory Structure

```
Keyhole-Beta/
├── core.py           # Core analysis logic and report generation
├── GUI.py            # CustomTkinter-based user interface
├── main.py           # Entry point
├── config/           # Stores presets and exclude lists
└── output reports/   # Automatically generated into user's OneDrive/Documents
```

## 📓 Example

Run the app, enter a URL like:

```
https://en.wikipedia.org/wiki/Natural_language_processing
```

Choose:
- Mode: `full`
- Summary size: `medium`

Then click **Run Analysis**. A report will be saved locally and shown in-app.

## 🧠 Powered By

- [Transformers (HuggingFace)](https://huggingface.co/transformers/)
- [VADER Sentiment](https://github.com/cjhutto/vaderSentiment)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [Textstat](https://github.com/shivam5992/textstat)
- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)

## 👨‍💻 Author

**Robert Franke**

Contact details available via the **About** tab in the app.

