# Module 11 Challenge: HTML Web Scraping

## Overview

This project is part of my **Data Analytics Bootcamp** coursework. It focuses on **web scraping** and **data analysis** to explore data from Mars-related sources. Using tools like **Splinter**, **Beautiful Soup**, and **Pandas**, I collected, organized, and visualized data, building foundational skills for data-driven decision-making.

---

## Contents

- [Project Objectives](#project-objectives)
- [Deliverables](#deliverables)
- [Setup](#setup)
- [Part 1: Mars News Titles and Previews](#part-1-mars-news-titles-and-previews)
- [Part 2: Mars Weather Data Analysis](#part-2-mars-weather-data-analysis)

---

## Project Objectives

1. **Scrape and Extract Data**:
   - Automate browsing and data extraction from websites using Splinter and Beautiful Soup.
   - Extract titles and preview texts of Mars news articles.
   - Scrape weather data from an HTML table on a Mars temperature webpage.

2. **Organize and Analyze Data**:
   - Store scraped data in Python data structures.
   - Analyze the data to answer questions about Mars weather patterns.

3. **Visualize and Communicate Findings**:
   - Create visualizations to demonstrate insights.
   - Export data to CSV for further use.

---

## Deliverables

### Deliverable 1: Scrape Titles and Previews from Mars News
- **Tool Used**: Jupyter Notebook (`part_1_mars_news.ipynb`)
- **Objective**: Scrape the Mars news website for titles and previews of articles.
- **Output**: Python list of dictionaries, optionally saved as a JSON file.

### Deliverable 2: Scrape and Analyze Mars Weather Data
- **Tool Used**: Jupyter Notebook (`part_2_mars_weather.ipynb`)
- **Objective**: Scrape weather data from the Mars temperature table.
- **Output**: Pandas DataFrame containing Mars weather data and visualizations.

---

## Setup

### Prerequisites

Ensure you have the following dependencies installed:

- Python 3.7+
- Jupyter Notebook
- Splinter
- Beautiful Soup
- Pandas
- Matplotlib

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/module-11-mars-web-scraping.git
   ```
2. Navigate to the project directory:
   ```bash
   cd module-11-mars-web-scraping
   ```
3. Install required libraries individually:
   ```bash
   pip install splinter beautifulsoup4 pandas matplotlib
   ```
4. Open the Jupyter notebooks:
   ```bash
   jupyter notebook
   ```

---

## Part 1: Mars News Titles and Previews

### Workflow

1. **Automate Browsing**:
   - Use Splinter to visit the Mars news site.
   - Inspect and identify HTML elements to scrape.

2. **Scrape Data**:
   - Use Beautiful Soup to extract article titles and preview text.
   - Store the results in a list of dictionaries:
     ```python
     [{'title': 'Title 1', 'preview': 'Preview 1'},
      {'title': 'Title 2', 'preview': 'Preview 2'}]
     ```

3. **Optional**:
   - Save the results to a JSON file for easy sharing.

---

## Part 2: Mars Weather Data Analysis

### Workflow

1. **Automate Browsing**:
   - Use Splinter to visit the Mars temperature data site.
   - Inspect the page and identify the HTML table elements.

2. **Scrape Data**:
   - Use Beautiful Soup to scrape the HTML table.
   - Convert the scraped data into a Pandas DataFrame.
   - Ensure appropriate column headings:
     - `id`, `terrestrial_date`, `sol`, `ls`, `month`, `min_temp`, `pressure`.

3. **Analyze Data**:
   - Convert data types (e.g., datetime, int, float).
   - Answer the following:
     - Number of months on Mars.
     - Number of Martian days recorded.
     - Coldest and warmest months (based on average minimum temperatures).
     - Months with lowest and highest atmospheric pressure.
     - Number of terrestrial days in a Martian year.

4. **Visualize Data**:
   - Create bar charts for temperature and pressure analyses.
   - Plot minimum daily temperatures to estimate the length of a Martian year.

5. **Export Results**:
   - Save the DataFrame to a CSV file.
