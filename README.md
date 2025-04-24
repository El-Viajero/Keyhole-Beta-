# 🔍 Keyh0le {Beta}

**Keyh0le {Beta}** is a desktop tool that allows users to analyze website content for keyword frequency, readability, sentiment, and automatic summarization. Built with a focus on simplicity and user experience, Keyh0le {Beta} combines NLP, sentiment analysis, and modern GUI design to provide rich insights from web pages.

## 🚀 Features

### 🔄 Updated & New Additions

- **Summarization**: Automatically condense full pages or sections using transformer-based models.
- **Sentiment Analysis**: Understand the tone of content with VADER sentiment scores.
- **Readability Metrics**: Includes Flesch Reading Ease scoring.
- **Keyword Extraction**: Displays the top 10 most frequent words, with optional exclusion filters.
- **Domain Crawling**: Recursively analyze multiple pages within a domain.
- **Named Entity Recognition (NER)** _(NEW)_: Identifies people, organizations, dates, and locations from content.
- **Configurable Presets**: Save and load excluded keyword sets.
- **Modern GUI**: A dark-themed interface built with `customtkinter`, now includes a Relationships tab and charting support.

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
  - `spacy`
  - `langdetect`
  - `validators`
  - `matplotlib`

Install dependencies:

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

## 🌟 Coming Soon

- **Entity Relationship Mapping** _(NEW)_: Maps relationships between co-occurring named entities in reports, viewable in a dedicated GUI tab.
- **Intelligence-Style Report Formatting** _(NEW)_: Reports are now structured with emoji-coded sections and grouped entities for clarity and readability.

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
- View named entity maps and structured summaries
- Load saved reports and explore relationships between entities

Reports are saved to your OneDrive `Documents/Reports` directory by default.

### New DLC Module (Drop-in Lightweight Components)

- **URL Validation**: Ensures valid input before analysis
- **Language Detection**: Warns if non-English content is detected
- **Named Entity Recognition**: Identifies structured entities in content
- **Common Word Chart**: Visualizes word frequency with a chart

### New Features Added

- **Full GUI integration for domain-wide crawling**
- **Named Entities now included in all report types**
- **Intelligence-style formatting** for professional reporting
- **Entity Relationship Mapping** in a new tab to uncover connections

## 📁 Directory Structure

```
Keyh0le {Beta}/
├── core.py             # Core analysis logic and report generation
├── GUI.py              # CustomTkinter-based user interface
├── main.py             # Entry point
├── DLC.py              # Lightweight feature integration helpers
├── ReportFormatter.py  # Structures and beautifies report output
├── RelationExtractor.py# Extracts entity relationships from reports
├── config/             # Stores presets and exclude lists
└── Reports/            # Output reports by type (Section, Full, Domain)
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
- [spaCy](https://spacy.io)
- [Langdetect](https://pypi.org/project/langdetect/)
- [Validators](https://pypi.org/project/validators/)

## 👨‍💻 Author

**Robert Franke**

Contact details available via the **About** tab in the app.
