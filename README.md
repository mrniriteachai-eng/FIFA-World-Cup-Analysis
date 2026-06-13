<div align="center">
  <a href="https://nirmalsaud.com.np">
    <img src="https://img.icons8.com/color/96/000000/code--v1.png" width="80" alt="Nirmal Saud Logo"/>
  </a>
  <h1>Nirmal Saud</h1>
  <p><a href="https://nirmalsaud.com.np">nirmalsaud.com.np</a></p>
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=32&pause=1000&color=00FF88&center=true&vCenter=true&width=800&height=100&lines=FIFA+World+Cup+Data+Analytics+Project;Python+%7C+Pandas+%7C+Matplotlib+%7C+NumPy;From+Raw+Data+To+Beautiful+Visualizations;Aspiring+AI+Engineer" alt="Typing Animation" />
</div>

<div align="center">
  <img src="https://img.shields.io/badge/STATUS-COMPLETED_SUCCESSFULLY-00FF88?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/PROJECT-FIFA_WORLD_CUP_ANALYSIS-FF0000?style=for-the-badge&logo=fifa&logoColor=white" />
  <img src="https://img.shields.io/badge/STACK-PYTHON_%7C_PANDAS_%7C_MATPLOTLIB-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/ASPIRING-AI_ENGINEER-FF6B6B?style=for-the-badge&logo=tensorflow&logoColor=white" />
</div>

<br/>

<div align="center">
  <a href="https://www.youtube.com/@MrNiriteach">
    <img src="https://img.shields.io/badge/SUBSCRIBE-@MrNiriteach-FF0000?style=for-the-badge&logo=youtube&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/nirmal-saud-a850193a0/">
    <img src="https://img.shields.io/badge/CONNECT-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/YOUR_USERNAME">
    <img src="https://img.shields.io/badge/FOLLOW-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://nirmalsaud.com.np">
    <img src="https://img.shields.io/badge/WEBSITE-nirmalsaud.com.np-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white" />
  </a>
</div>

---

## Project Overview

This is my signature data analytics project that showcases my skills in:

- Data Manipulation with Pandas
- Numerical Computing with NumPy
- Data Visualization with Matplotlib
- Real-World Analysis - FIFA World Cup (2014-2026)

The Mission: Turn raw football data into actionable insights, beautiful charts, and tell a story through numbers.

---

## What This Project Does

| Feature | Description | Output |
|---------|-------------|--------|
| Top Goal Scorers | Calculates total goals per country (Home + Away) | Top 10 Teams List |
| Bar Chart | Visualizes top 10 goal-scoring nations | goals_chart.png |
| Pie Chart | Shows goal distribution among top 5 teams | top5_pie.png |
| Win Analysis | Counts Home Wins vs Away Wins vs Draws | Stats + Bar Chart |
| Year-wise Analysis | Matches played in each World Cup year | years_chart.png |
| Match Results Chart | Visual comparison of match outcomes | results_chart.png |

---

## Code Breakdown (Learn How It Works)

### 1. Import Libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
pandas is imported for data manipulation. matplotlib.pyplot is imported for creating charts.

2. Load the Data
python
df = pd.read_csv('world_cup_data.csv')
Reads the CSV file and converts it into a pandas DataFrame.

3. Year Analysis
python
year_counts = df['Year'].value_counts().sort_index()
Selects the Year column, counts each year's occurrences, and sorts chronologically.

4. Goal Calculation
python
goals_home = df.groupby('Home Team')['Home Team Goals'].sum()
goals_away = df.groupby('Away Team')['Away Team Goals'].sum()
total_goals = goals_home.add(goals_away, fill_value=0).sort_values(ascending=False)
Groups matches by team name, sums goals for home and away matches, then combines both totals.

5. Win Analysis
python
home_wins = (df['Home Team Goals'] > df['Away Team Goals']).sum()
away_wins = (df['Away Team Goals'] > df['Home Team Goals']).sum()
draws = (df['Home Team Goals'] == df['Away Team Goals']).sum()
Creates boolean comparisons and counts True values to determine wins and draws.

6. Visualization Pipeline
python
plt.figure(figsize=(14, 6))
total_goals.head(10).plot(kind='bar', color='#FF6B6B')
plt.title('Top 10 Teams - Total Goals')
plt.savefig('goals_chart.png')
plt.show()
Creates bar chart showing top 10 goal-scoring teams with custom styling.

Project Structure
text
FIFA_World_Cup_Project/
│
├── world_cup_data.csv          # Dataset (2014-2026 matches)
├── analysis.py                 # Main Python script
│
├── goals_chart.png             # Bar chart output
├── top5_pie.png                # Pie chart output
├── results_chart.png           # Wins/Draws chart
├── years_chart.png             # Year distribution
│
└── README.md                   # Project documentation
How to Run This Project
Prerequisites
bash
pip install pandas matplotlib numpy
Steps
bash
git clone https://github.com/YOUR_USERNAME/fifa-world-cup-analysis.git
cd fifa-world-cup-analysis
python analysis.py
Sample Console Output
text
============================================================
FIFA WORLD CUP DATA ANALYSIS (2014-2026)
============================================================

Matches by Year:
2006    4
2010    3
2014    5
2018    12
2022    14
2026    8

TOP 10 TEAMS - TOTAL GOALS:
Brazil      28
Germany     28
France      20
Spain       18
Italy       15
Argentina   12
Netherlands 10
England      9
Portugal     8
Belgium      7

MATCH RESULTS (All Time):
Home Wins: 28
Away Wins: 12
Draws: 8

Analysis Complete!
Charts saved: goals_chart.png, top5_pie.png, results_chart.png, years_chart.png
Generated Files Description
File Name	Type	Description
goals_chart.png	Bar Chart	Shows top 10 goal-scoring teams
top5_pie.png	Pie Chart	Shows goal share among top 5 teams
results_chart.png	Bar Chart	Compares home wins, away wins, draws
years_chart.png	Bar Chart	Shows matches played per year
What I Learned From This Project
Skill	How I Used It
Pandas GroupBy	Aggregated goals by country
Boolean Filtering	Counted wins using comparison
Matplotlib Styling	Custom colors, grid lines, labels
Data Storytelling	Transformed numbers into insights
Git/GitHub	Version control and project sharing
Future Improvements
Add data from all World Cup years (1930-2022)

Create interactive dashboard using Plotly

Implement machine learning to predict match winners

Add player-level statistics (top scorers, assists)

Connect With Me
Platform	Link
Website	nirmalsaud.com.np
YouTube	@MrNiriteach
LinkedIn	Nirmal Saud
GitHub	github.com/YOUR_USERNAME
Roadmap for Aspiring AI Engineer
Current: FIFA Analysis
Next: More Datasets
Then: Advanced Visualization
Then: Machine Learning
Then: Deep Learning
Goal: AI Engineer

What's Next:

Add more World Cup years (1950-2026)

Create interactive dashboards with Plotly

Predict match winners using ML

Build a recommendation system for teams

Support
If you find this project helpful:

Star this repository on GitHub

Subscribe to my YouTube channel

Share with fellow learners

License
This project is open-source and free to use for educational purposes.

<div align="center"> <p>Made with love by Nirmal Saud</p> <p><a href="https://nirmalsaud.com.np">nirmalsaud.com.np</a></p> <p>Last Updated: 2024</p> <p>Keep coding. Keep learning. Keep growing.</p> </div> ```
