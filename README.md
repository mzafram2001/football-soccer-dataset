# ⚽️ football-database-fver

![Status](https://img.shields.io/badge/Status-Free-orange)
![License](https://img.shields.io/badge/License-CC_BY_NC-blue)
![Format](https://img.shields.io/badge/Format-SQL_CSV_JSON-green)
![Version](https://img.shields.io/badge/Version-v20251231-purple)

> [!CAUTION]
> **Disclaimer:** Data is collected from public sources. This repository is for educational and research purposes only. Not financial advice.

> [!TIP]
> **Want to help?**
> ⭐ Do you like this project? If you find this data useful, please give it a Star! It helps me keep updating it.

---

## 📖 About
Free and open-source football database containing historical and current match statistics, results, and betting odds. Ideal for data analysis, machine learning models, and football apps.

The data covers major leagues and includes detailed metrics like possession, shots, cards, corners, and betting odds (Bet365).

## 📊 Data Sample
Here is a preview of the main dataset structure (columns selected for readability).
> **Note:** The actual CSV contains **34 columns** including detailed betting odds and formation IDs.

```csv
id, codification, season_id, date, round, home_id, away_id, home_formation_id, away_formation_id, home_goals_full_time, away_goals_full_time, home_goals_half_time, away_goals_half_time, result, home_possession, away_possession, home_shots, away_shots, home_shots_on_target, away_shots_on_target, home_fouls, away_fouls, home_yellow_cards, away_yellow_cards, home_red_cards, away_red_cards, home_corners, away_corners, home_offsides, away_offsides, b365h_odds, b365d_odds, b365a_odds, competition_code
3940, 21/08/2015_Málaga_Sevilla, 6, 21/08/2015, 1, 28, 12, 1, 3, 0, 0, 0, 0, D, 58, 42, 25, 10, 5, 2, 19, 11, 3, 5, 0, 1, 7, 2, 1, 3, 3.40, 3.40, 2.15, LAL
3941, 22/08/2015_Deportivo-La-Coruña_Real-Sociedad, 6, 22/08/2015, 1, 29, 11, 3, 1, 0, 0, 0, 0, D, 58, 42, 16, 9, 5, 2, 16, 10, 3, 2, 0, 0, 5, 4, 2, 2, 2.50, 3.20, 3.00, LAL
3942, 22/08/2015_Espanyol_Getafe, 6, 22/08/2015, 1, 17, 6, 3, 3, 1, 0, 1, 0, H, 34, 67, 5, 13, 2, 3, 19, 14, 2, 5, 0, 1, 4, 6, 5, 2, 1.91, 3.40, 4.33, LAL
3943, 22/08/2015_Atlético-Madrid_Las-Palmas, 6, 22/08/2015, 1, 3, 18, 1, 9, 1, 0, 1, 0, H, 62, 38, 14, 8, 3, 1, 11, 16, 2, 0, 0, 0, 4, 4, 0, 0, 1.20, 6.50, 15.00, LAL
3944, 22/08/2015_Rayo-Vallecano_Valencia, 6, 22/08/2015, 1, 15, 13, 1, 2, 0, 0, 0, 0, D, 53, 47, 8, 10, 3, 4, 19, 11, 3, 1, 0, 0, 3, 3, 0, 1, 3.60, 3.50, 2.05, LAL
```

> [📂 View full CSV file](data/csv/results.csv)

## 🗂 Column Dictionary
Brief explanation of the key columns available in the dataset:

* **Match Info:** `date`, `season_id`, `round`, `competition_code`.
* **Teams:** `home_id`, `away_id` (Relational IDs), `home_formation_id`, `away_formation_id`.
* **Score:**
    * `home_goals_full_time` / `away_goals_full_time` (Final Score).
    * `home_goals_half_time` / `away_goals_half_time` (Half Time Score).
    * `result`: **H** (Home Win), **A** (Away Win), **D** (Draw).
* **Stats:** Possession, Shots (Total/On Target), Fouls, Corners, Offsides.
* **Cards:** Yellow and Red cards for both teams.
* **Odds (Bet365):** `b365h_odds` (Home), `b365d_odds` (Draw), `b365a_odds` (Away).

## 🚀 How to use
You can clone the repository or download the specific format you need:

1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/tu-usuario/football-database-fver.git](https://github.com/tu-usuario/football-database-fver.git)
    ```
2.  **Import Data:**
    * **CSV:** Ready for Pandas/Excel in `/data/csv/`.
    * **SQL:** Import scripts available in `/data/sql/`.
    * **JSON:** Structured data in `/data/json/`.

---
*Created by Miguel Zafra*
