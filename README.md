# 🎮 Steam Games Market & Genre Trend Analysis (2004–2024)

An exploratory data analysis (EDA) and text mining project examining top-performing games on Steam, release trends across two decades, genre dominance, player mechanics preferences, and market dynamics.

## 📌 Project Overview

This project analyzes historical and contemporary data from Steam's top-performing titles (covering sales, revenue, and player reviews) spanning from **November 2004 to September 2024**. The objective is to uncover patterns in game release frequency, popular gameplay tags, commercial recency biases, player engagement drivers, and textual keyword features.

### Key Objectives

* **Temporal Trend Analysis:** Track the evolution of game releases from 2004 to 2024.
* **Genre & Tag Breakdown:** Dissect core game genres vs. descriptive feature tags (`Action`, `Multiplayer`, `Co-op`, `First-Person`).
* **Market Dynamics:** Evaluate the commercial dominance of modern releases (recency bias) and social/multiplayer experiences.
* **Data Cleaning & Tag Explosion:** Process multi-label string representations into exploded lists for precise aggregation.
* **Text Feature Mining:** Extract frequency patterns and key text attributes using n-gram vectorization and stop-word filtering.

## 🔑 Key Insights

1. **Exponential Growth in Modern Era (2020–2024):**
   * Over **75% of games** in the top-chart dataset were released after August 2017 (median: January 2021).
   * Releases across top categories surged dramatically from 2022, peaking in **2024**.
   * *Catalog Recency Bias:* This spike highlights how recent titles heavily dominate Steam's top sales, revenue, and engagement rankings.

2. **Dominance of Social & Connected Gameplay:**
   * **`Multiplayer`** emerged as the single fastest-growing gameplay mode, climbing from 14 games (2022) to **34 releases in 2024**.
   * **`Co-op`** (21 releases in 2024) and **`Online Co-Op`** (20 releases in 2024) followed identical trajectories, confirming social multiplayer mechanics as major commercial drivers.

3. **`Action` as the Core Genre Backbone:**
   * **`Action`** remains the premier core genre tag, maintaining steady multi-year growth and reaching **24 releases in 2024**. It frequently pairs with first-person and multiplayer tags.

4. **Expansion of Immersive Perspectives:**
   * **`First-Person`** titles nearly doubled in 2024 (**14 releases**), showing renewed commercial momentum for FPS and immersive action games.

*Note: 2024 data captures releases through September 26, 2024, excluding Q4 holiday releases.*

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.10+
* **Data Manipulation:** `pandas`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Text Mining & NLP:** `scikit-learn` (`CountVectorizer`)
* **Data Parsing:** `ast` (Python Standard Library)
* **Environment:** Jupyter Notebook / Visual Studio Code

## 📊 Dataset Summary

* **Scope:** 290 unique top-chart games on Steam.
* **Exploded Tag Attributes:** ~5,507 record entries spanning 350 unique genre/feature labels.
* **Time Range:** November 2004 – September 2024.

## 📁 Repository Structure

```
├── datasets/                     # Local dataset folder (ignored by Git; download from Kaggle)
│   ├── games_description.csv     # Game metadata, genres, and release dates
│   ├── games_ranking.csv         # Top sales, revenue, and review rankings
│   └── steam_game_reviews.csv    # User review texts and sentiment labels
├── .gitignore                    # Excludes large dataset files and local environments
├── notebook.ipynb                # Main EDA and text-mining Jupyter Notebook
├── README.md                     # Project documentation and key findings
└── requirements.txt              # Python package dependencies
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/riowinarno/steam-games-reviews-and-rankings.git
cd steam-games-reviews-and-rankings
```

### 2. Set Up Virtual Environment & Install Dependencies

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Launch the Jupyter Notebook

```bash
jupyter notebook notebook.ipynb
```

## 🤝 License & Acknowledgments

This project is open-source and available under the [MIT License](LICENSE). Data collected from Steam public store metrics and community tags.