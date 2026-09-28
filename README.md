# 🎬 Netflix Titles — Exploratory Data Analysis

An end-to-end exploratory data analysis of the Netflix catalog (8,807 titles, 12 columns) using Python. The project covers data cleaning, feature engineering, and 9 Netflix-themed visualizations that reveal how the platform's content is distributed and how it has evolved over time.

## 📌 Project Overview

The goal is to answer practical questions about Netflix's library:

- What is the split between Movies and TV Shows?
- Which countries and genres dominate the catalog?
- When was most of the content added to the platform?
- What are typical movie lengths and show sizes?
- How is content distributed across maturity ratings?

## 📂 Dataset

- **File:** `netflix_titles.csv`
- **Records:** 8,807 titles
- **Columns:** 12 (type, title, director, cast, country, date_added, release_year, rating, duration, listed_in, description, show_id)
- **Source:** [Netflix Movies and TV Shows – Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

## 🧹 Data Cleaning & Feature Engineering

- Converted `date_added` to datetime and extracted `year_added`, `month_added`, `month_name`
- Extracted `duration_min` for movies and `seasons` for TV shows from the `duration` column
- Fixed misclassified values in `rating` (rows containing durations such as "74 min")
- Split multi-value columns (`country`, `listed_in`) into individual rows for accurate counting
- Assessed missing values in `director`, `cast`, and `country`

## 📊 Visualizations

1. Content type distribution (Movies vs TV Shows)
2. Content added per year
3. Top 15 production countries
4. Top 15 genres
5. Content rating distribution
6. Movie duration (histogram + box plot)
7. Number of seasons per TV show
8. Release year distribution
9. Monthly content additions

## 🔑 Key Findings

| Insight | Finding |
|---|---|
| Content split | 69.6% Movies, 30.4% TV Shows |
| Top country | United States (3,689 titles) |
| Top genre | International Movies |
| Most common rating | TV-MA (mature audience) |
| Average movie length | ~99 minutes |
| Peak addition years | 2019 – 2020 |
| Oldest / newest title | 1925 / 2021 |

## 🛠️ Tech Stack

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/netflix-titles-data-analysis.git
cd netflix-titles-data-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Place netflix_titles.csv in the project folder, then launch
jupyter notebook netflix_analysis.ipynb
```

## 📁 Repository Structure

```
├── netflix_analysis.ipynb   # Full analysis notebook
├── netflix_titles.csv       # Dataset
└── README.md
```

## 👤 Author

**Mohammed Akram Anwar**
Artificial Intelligence Engineering Technologies Student — Northern Technical University

- LinkedIn: [your-link]
- GitHub: [@your-username]

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
