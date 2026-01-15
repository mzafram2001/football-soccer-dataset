# ⚽️ football-soccer-dataset (Free Sample)

![Status](https://img.shields.io/badge/Status-Free_Sample-orange)
![License](https://img.shields.io/badge/License-CC_BY_NC-blue)
![Format](https://img.shields.io/badge/Format-CSV%20%7C%20JSON-green)
![Version](https://img.shields.io/badge/Version-v20260115-purple)

## 📖 About this dataset
This repository contains a **free sample** of historical football (soccer) match results, specifically curated for **data science, machine learning models, and sports betting analytics**.

The data is cleaned, normalized, and ready to be loaded into **Python (Pandas), R,** or **Excel**.

> **⚠️ Note:** This is a **static demo** repository. The data contained here is **NOT** automatically updated.

## 📂 Data Dictionary
The file `data/sample_laliga.csv` includes the following columns:

* `Date`: Match Date (DD/MM/YYYY).
* `HomeTeam`: Name of the home team.
* `AwayTeam`: Name of the away team.
* `FTHG`: Full Time Home Goals.
* `FTAG`: Full Time Away Goals.
* `FTR`: Full Time Result (**H**=Home Win, **D**=Draw, **A**=Away Win).
* `HS` / `AS`: Home/Away Shots.
* `HST` / `AST`: Home/Away Shots on Target.
* *(Add any other specific columns you have here, e.g., 'B365H' for betting odds)*

## 💻 Usage Example (Python / Pandas)
You can load this dataset directly into your environment without downloading the file:

```python
import pandas as pd

# Load the dataset directly from GitHub
url = "[https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/data/sample_laliga.csv](https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/data/sample_laliga.csv)"
df = pd.read_csv(url)

# Example: Check who won the most home games
home_wins = df[df['FTR'] == 'H']['HomeTeam'].value_counts()
print(home_wins.head())


## 🚀 Free vs. Premium: Why upgrade?
To support the maintenance of this project, we offer a **Premium Repository** that is automatically updated every week with the latest match results and odds.

| Feature | 🆓 Free Version (This Repo) | ⚡ Premium Version (Sponsors) |
| :--- | :---: | :---: |
| **History Depth** | Sample Season (e.g., 2018-2019) | **Full History (2015 - Present)** |
| **Updates** | Static (Never updated) | **Automatic (Weekly/Daily)** |
| **Coverage** | Single League Demo | **Top 10+ Major Leagues** |
| **Data Types** | Basic Results | **+ Betting Odds & Match Stats** |
| **Access** | Public | **[Become a Sponsor to Access]** |

👉 **[GET FULL ACCESS & AUTOMATIC UPDATES HERE](YOUR_PATREON_OR_SPONSORS_LINK)**
