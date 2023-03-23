# BBC News Web Scraper

This repository contains a Python-based web scraper for extracting article content from BBC News articles. The web scraper can extract the title, date published, and the main content of an article.

## Table of Contents

- [Features](#features)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [License](#license)

## Features

- Extracts the article title, date published, and main content from a BBC News article URL
- Returns the extracted information in JSON format
- Includes functions to extract entities such as people, places, and organizations from the extracted content
- Comes with a test suite for validating the functionality of the web scraper and entity extraction

## Dependencies

- Python 3.6 or higher
- BeautifulSoup4
- Requests
- (Optional) Spacy, if using entity extraction

## Installation

1. Clone the repository:

git clone https://github.com/your_username/bbc-news-web-scraper.git


## Usage

1. Import the `bbc_scraper` function from the `scraper.py` module:

```python
from scraper import bbc_scraper
```

Call the bbc_scraper function with a BBC News article URL:

```python
url = 'https://www.bbc.co.uk/news/uk-51004218'
article_data = bbc_scraper(url)
```

(Optional) If you want to extract entities from the article content, you can use the extract_entities function:

```python
from scraper import extract_entities

content = article_data["Content"]
entities = extract_entities(content)
```
## Testing

The repository includes a test suite for validating the functionality of the web scraper and entity extraction. To run the tests, execute the following command:

## License
This project is licensed under the MIT License.
