<div align="center">

# 🏏 IPL Analysis Dashboard

### End-to-End Excel BI Project | Power Pivot · Star Schema · DAX · Interactive Slicers

<br>

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Pivot](https://img.shields.io/badge/Power_Pivot-Enabled-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-Measures-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=for-the-badge)
![Sheets](https://img.shields.io/badge/Sheets-9_Tabs-purple?style=for-the-badge)

<br>

> **"Not just charts — a fully relational BI solution built entirely in Excel."**

</div>

----

## 🎯 What This Project Does

This project transforms raw IPL match data into a **fully interactive analytics dashboard** — built entirely in Excel using enterprise-grade techniques:

- 📐 **Star Schema** data model (same pattern used in data warehouses)
- ⚡ **Power Pivot** for handling relationships across multiple tables
- 🧮 **DAX measures** for dynamic KPI calculations
- 🎛️ **Slicers** for real-time cross-dashboard filtering
- 📊 **Pivot Charts** — bar, line, pie, and combo charts

---

## 📊 Dashboard 1 — Team Performance

<table>
<tr>
<td>

### 📌 KPI Cards
| Metric | Value |
|---|---|
| 🎮 Total Matches | **60** |
| 🏟️ Total Teams | **9** |
| 🏏 Total Runs | **20,944** |
| 🎳 Total Wickets | **799** |

</td>
<td>

### 📌 Charts Included
- 📊 Team vs Wins
- 📊 Team vs Total Runs
- 🏟️ Venue vs Matches
- 🥧 Win Type — By Runs vs By Wickets

</td>
</tr>
</table>

🎛️ **Slicers:** Venue Name · Team Name

---

## 📊 Dashboard 2 — Player Performance

<table>
<tr>
<td>

### 📌 KPI Cards
| Metric | Value |
|---|---|
| ⚡ Avg Strike Rate | **106.7** |
| 💰 Economy | **613.4** |

</td>
<td>

### 📌 Charts Included
- 📈 Player vs Total Runs
- 📈 Player vs Total Wickets
- 📊 Player Strike Rate (Combo Chart)
- 🥧 Player Economy Breakdown

</td>
</tr>
</table>

🎛️ **Slicers:** Venue Name · Player Name

---

## 🗂️ Data Architecture — Star Schema

```
                     ┌──────────────┐
                     │  dim_venue   │
                     │  (Stadiums)  │
                     └──────┬───────┘
                            │
┌─────────────┐    ┌────────┴────────┐    ┌──────────────┐
│  dim_team   │────│   fact_match    │────│  dim_player  │
│  (9 Teams)  │    │  (Match Stats)  │    │  (Players)   │
└─────────────┘    └────────┬────────┘    └──────┬───────┘
                            │                    │
                     ┌──────┴───────┐            │
                     │ fact_player  │────────────┘
                     │(Player Stats)│
                     └─────────────┘
```

| Table | Type | Columns |
|---|---|---|
| `fact_match` | ⚙️ Fact | match_id, team_id, venue_id, runs, wickets, win_type |
| `fact_player` | ⚙️ Fact | player_id, match_id, runs, wickets, strike_rate, economy |
| `dim_team` | 📋 Dimension | team_id, team_name |
| `dim_player` | 📋 Dimension | player_id, player_name |
| `dim_venue` | 📋 Dimension | venue_id, venue_name |

> ✅ **Zero VLOOKUPs.** All relationships are defined inside the **Power Pivot Data Model** — exactly how it's done in enterprise BI.

---

## 🔍 Key Insights Uncovered

```
🏆  CSK & SRH          →  Lead all teams in total wins
🏏  Top Batter          →  982 runs in a single season
🎳  Top Bowler          →  25 wickets — nearly 2x the next best
🏟️  Wankhede Stadium   →  Highest number of matches hosted
📊  Win Pattern         →  Majority of wins are by RUNS, not wickets
⚡  Strike Rate         →  Average 106.7 — high-scoring edition confirmed
```

---

## ⚙️ Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| 📁 Data Storage | Excel Tables | Structured raw data |
| 🔗 Data Modeling | Power Pivot | Relationships across fact & dim tables |
| 🧮 Calculations | DAX | KPI measures, aggregations |
| 📊 Visualization | Pivot Charts | Interactive bar, line, pie, combo charts |
| 🎛️ Interactivity | Slicers | Cross-dashboard real-time filtering |

---

## 💡 Why This Is Different From a Basic Excel Dashboard

| Basic Excel Dashboard | This Project |
|---|---|
| VLOOKUP to join data | Power Pivot relationships |
| Hardcoded values | DAX dynamic measures |
| Single flat table | Star Schema (fact + dimension tables) |
| Static charts | Fully interactive Pivot Charts + Slicers |
| One sheet | 9 organized sheets with clean architecture |

> This project mirrors how **real BI tools like Power BI and Tableau** handle data — just built entirely in Excel.

---

## 🚀 How to Run This Project

```
1. Download IPL_Analysis_Dashboard.xlsx
2. Open in Microsoft Excel 2016 or later (Office 365 recommended)
3. Click "Enable Content" when prompted — required for Power Pivot
4. Go to "Team Performance Dashboard" or "Player Performance Dashboard" tab
5. Use the slicers to filter by Venue, Team, or Player — all charts update live
```

---

## 📁 Repository Structure

```
📦 IPL-Analysis-Dashboard-Excel
 ┣ 📊 IPL_Analysis_Dashboard.xlsx     ← Main workbook
 ┣ 📁 screenshots/
 ┃  ┣ 🖼️  team_dashboard.png
 ┃  ┗ 🖼️  player_dashboard.png
 ┗ 📄 README.md
```

---

## 👤 About Me

**Raushan Kumar** — Final Year B.Tech CSE Student at RGPV University, Bhopal

I'm passionate about turning raw data into clear, actionable insights. Currently seeking **Data Analyst / Business Analyst** opportunities where I can apply skills in Excel, Python, SQL, and BI tools.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/raushankumar999)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github)](https://github.com/Raushan792)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-8A2BE2?style=for-the-badge&logo=netlify&logoColor=white)](https://raushan-kumar-01.netlify.app)

</div>

----

<div align="center">

⭐ **If this project impressed you, give it a star — it motivates me to build more!** ⭐

</div>
