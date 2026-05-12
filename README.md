# Sentiment-Analysis-of-the-US-Israel-Iran
Real-time sentiment analysis &amp; topic modeling of the US/Israel–Iran conflict using live data from BBC, Al Jazeera, Reuters, RT News, Google News, Reddit, and YouTube.


![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=flat&logo=flask)
![NLP](https://img.shields.io/badge/NLP-VADER%20%7C%20LDA-8B5CF6?style=flat)
![Data](https://img.shields.io/badge/Data-Live%20RSS%20%7C%20Reddit%20%7C%20YouTube-EF4444?style=flat)

## War Sentiment Analysis — US/Israel–Iran Conflict

A real-time NLP dashboard that collects, processes, and visualises 
sentiment across international news coverage and social media commentary 
on the US/Israel–Iran conflict.

### What it does
- Pulls live articles from 14 RSS feeds (BBC, Al Jazeera, Reuters, 
  RT News, Google News, Sky News, Guardian, DW, France 24) plus 
  direct web scraping, Reddit PRAW, and YouTube Data API v3
- Runs a full NLP pipeline: HTML stripping → tokenisation → 
  stopword removal → VADER sentiment scoring
- Performs LDA topic modelling (gensim) across 7 conflict themes
- Classifies every article into one of five thematic angles: 
  Military Operations, Geopolitical Tensions, Economic Impact, 
  Media Narratives, and Support for War
- Displays results in a live dashboard with Chart.js visualisations 
  that update on every refresh

### Tech stack
| Layer      | Tools |
|------------|-------|
| Backend    | Python, Flask, feedparser, BeautifulSoup, PRAW |
| NLP        | VADER, gensim LDA, NLTK, pandas |
| Frontend   | HTML/CSS, Vanilla JS, Chart.js |
| Data       | RSS, web scraping, Reddit API, YouTube Data API v3 |
| Export     | openpyxl (4-sheet Excel workbook) |

### Key findings
Coverage of the conflict skews predominantly negative across all 
outlets (consistent with conflict reporting norms), with RT News 
and Al Jazeera showing statistically different framing compared 
to Western sources. Economic Impact articles carry the most 
negative average compound scores, while Diplomatic Relations 
articles trend closest to neutral.

