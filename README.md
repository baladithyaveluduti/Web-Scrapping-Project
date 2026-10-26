# Web-Scrapping-Project
Movie Rating Analysis 
# 🎬 TMDB Top Rated Movies — Web Scraping & Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project focuses on **web scraping and exploratory data analysis (EDA)** using the [TMDB (The Movie Database)](https://www.themoviedb.org/movie/top-rated) Top Rated Movies page.

The project collects movie information from TMDB, cleans and preprocesses the extracted data, and performs exploratory analysis using Python. Visualizations are created to understand movie ratings, genres, release decades, runtime, directors, budgets, and revenue.

The main objective is to identify patterns and insights among top-rated movies through data-driven analysis.

## 🎯 Objectives

- Extract movie information from the TMDB website using web scraping.
- Collect movie details from multiple pages.
- Clean and preprocess the scraped dataset.
- Perform exploratory data analysis using Pandas and NumPy.
- Visualize trends and relationships between movie attributes.
- Answer business questions related to movie ratings, genres, budgets, and revenue.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Selenium** — Browser automation and webpage access
- **BeautifulSoup** — HTML parsing and data extraction
- **Requests** — HTTP requests
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualizations
- **Jupyter Notebook** — Interactive development environment

## 🌐 Data Source

**Website:** [TMDB Top Rated Movies](https://www.themoviedb.org/movie/top-rated)

The notebook is designed to scrape up to **500 movie records** by processing up to 25 pages, with approximately 20 movies per page, and then visit individual movie pages to collect additional details.

## 📊 Dataset Description

The scraped dataset includes the following columns:

| Column | Description |
|---|---|
| Rank | Position in the scraped movie list |
| Title | Movie title |
| Release_Date | Movie release date |
| Rating | TMDB movie rating |
| Genre | Movie genres |
| Director | Movie director |
| Runtime | Movie duration |
| Certificate | Movie certification |
| Language | Original movie language |
| Budget | Movie production budget |
| Revenue | Total movie revenue |
| Overview | Short movie description |
| Link | URL of the movie page |

The notebook also creates additional features for analysis, including release year, decade, main genre, movie length category, budget category, and rating category.

## ⚙️ Project Workflow

### 1. Web Scraping
- Access the TMDB Top Rated Movies page using Selenium.
- Parse webpage HTML using BeautifulSoup.
- Extract movie titles, release dates, ratings, overviews, and links.
- Visit individual movie pages to collect additional movie details.

### 2. Data Collection
- Scrape multiple pages of movie listings.
- Combine the collected information into a Pandas DataFrame.
- Assign ranks to the scraped movies.
- Export the collected dataset to `Scraped.csv`.

### 3. Data Cleaning and Preprocessing
- Check for missing values and duplicate records.
- Remove records without movie titles.
- Clean and standardize relevant columns.
- Convert numerical fields into appropriate data types.
- Create derived columns for further analysis.

### 4. Exploratory Data Analysis
Analyze the distribution of ratings, movie genres, release decades, runtimes, and languages. Compare ratings across directors and decades, and investigate relationships between runtime, budget, revenue, and ratings.

### 5. Data Visualization
Create charts to present findings clearly and identify patterns in the dataset.

## 📈 Visualizations Performed

The notebook includes the following visual analyses:

1. **Rating Distribution** — Understand the distribution of movie ratings.
2. **Movies per Decade** — Compare the number of top-rated movies released across decades.
3. **Top 10 Genres** — Identify the most frequently appearing genres.
4. **Runtime Distribution** — Analyze the duration of movies.
5. **Original Language Analysis** — Identify the most common movie languages.
6. **Average Rating by Decade** — Compare average movie ratings across decades.
7. **Director Comparison** — Compare average ratings for directors with multiple movies.
8. **Runtime vs. Rating** — Explore the relationship between movie duration and rating.
9. **Budget vs. Revenue** — Examine the relationship between production budgets and revenue.
10. **Correlation Heatmap** — Analyze correlations between year, runtime, rating, budget, and revenue.
11. **Genre-Based Comparison** — Compare runtime and ratings across selected genres.
12. **Blockbuster Genre Analysis** — Explore genres among movies in the notebook's high-budget category.

## 💡 Business Questions Answered

The analysis investigates questions such as:

- Which movie has the highest rating in the scraped dataset?
- Which decade contains the most top-rated movies?
- Which decade has the highest average rating, considering a minimum number of movies?
- What are the average, median, minimum, and maximum movie ratings?
- What are the average, shortest, and longest movie runtimes?
- Which movie certificate is most common?
- Which genre appears most frequently?
- Which original language is most common?
- Which directors have the most movies in the dataset?
- How many movies have a runtime greater than 150 minutes?
- Do movies longer than 150 minutes have higher average ratings?
- Do movies in different budget categories receive different average ratings?
- Which movie has the highest revenue?
- Which movie has the highest calculated profit?
- Which genres are most common among the highest-rated movies?

## 📁 Project Structure

```text
TMDB-Web-Scraping-EDA/
│
├── WEBSCRAPPING PROJ.ipynb
├── Scraped.csv
└── README.md
```

`Scraped.csv` is generated when the relevant export cell in the notebook is executed.

## 🚀 How to Run the Project

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Google Chrome installed
- A compatible Selenium WebDriver setup

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
cd TMDB-Web-Scraping-EDA
```

### Step 2: Install the Required Libraries

```bash
pip install requests beautifulsoup4 selenium pandas numpy matplotlib seaborn jupyter
```

### Step 3: Open Jupyter Notebook

```bash
jupyter notebook
```

Open `WEBSCRAPPING PROJ.ipynb` and execute the cells in order.

**Note:** The notebook uses Selenium to access TMDB pages. Website structure, access restrictions, or changes to HTML elements may affect scraping results. Ensure that your browser and Selenium setup are compatible.

## 🔍 Key Learnings

- Understanding the fundamentals of web scraping.
- Extracting structured information from HTML pages.
- Using Selenium for browser automation.
- Cleaning and preprocessing real-world data.
- Performing exploratory data analysis with Pandas and NumPy.
- Creating meaningful visualizations with Matplotlib and Seaborn.
- Comparing movie attributes and interpreting statistical relationships.
- Translating analysis into answers to practical business questions.

## ⚠️ Limitations

- The number of successfully collected movies may vary depending on website availability and scraping success.
- Some movie details, such as budget and revenue, may be missing or unavailable.
- Correlation does not necessarily indicate causation.
- Movie ratings and website content can change over time.
- Findings represent the scraped dataset and should not automatically be generalized to all movies.

## 👨‍💻 Conclusion

This project demonstrates an end-to-end beginner-friendly data analysis workflow, from collecting data from a real-world website to cleaning, exploring, and visualizing the results.

By combining web scraping with exploratory data analysis, the project helps uncover patterns in top-rated movies and develops practical skills in Python-based data analytics.

## 📜 Disclaimer

This project is intended for educational and portfolio purposes. TMDB owns its website content and associated data. Please respect the website's terms of use, applicable policies, and rate limits when collecting data.

---

**Skills:** Python | Web Scraping | Selenium | BeautifulSoup | Pandas | NumPy | EDA | Data Visualization | Matplotlib | Seaborn
