---
slug: github-hugo-rss-mysql-update-note-technical-overview
id: github-hugo-rss-mysql-update-note-technical-overview
title: hugo-rss-mysql-update
repo: justin-napolitano/hugo-rss-mysql-update
githubUrl: https://github.com/justin-napolitano/hugo-rss-mysql-update
generatedAt: '2025-11-24T18:38:27.692Z'
source: github-auto
summary: >-
  This repo automates scraping RSS feeds from a Hugo blog and updates a MySQL
  database with new posts. It simplifies RSS parsing while ensuring a persistent
  data store.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repo automates scraping RSS feeds from a Hugo blog and updates a MySQL database with new posts. It simplifies RSS parsing while ensuring a persistent data store.

### Key Features
- Extracts post metadata from RSS feeds
- Converts dates to epoch timestamps
- Tracks last run timestamps to prevent duplication
- Connects to MySQL using environment-configured credentials

### Tech Stack
- Python 3
- `feedparser` for parsing RSS
- `mysql-connector-python` for MySQL access
- `dotenv` for managing environment variables

### Quick Start

#### Prerequisites
- Python 3
- Accessible MySQL server

#### Installation
```bash
git clone https://github.com/justin-napolitano/hugo-rss-mysql-update.git
cd hugo-rss-mysql-update
python3 -m venv venv
source venv/bin/activate
pip install feedparser mysql-connector-python python-dotenv
```

#### Configuration
Create a `.env` file with your database credentials.

#### Running
Test the connection:
```bash
python db-connector.py
```
Run the scraper:
```bash
python rss-scraper.py
```

Watch out for required DB setup and environment configurations.
