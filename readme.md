# Bundesliga data Exploration
## by Frederik Riess


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

The dataset is a collection of the latest 16 Bundesliga (German national Football League) seasons. I read those 16 .csv-files and created one single dataframe. In this dataframe are listed all matches from those 16 seasons (overall 4356 matches). Since there are many other parameters (most of the time betting odds) included, I just kept the ones I am interested in for my analysis. The single dataframe is also saved as a .csv-file ('bundesliga_data.csv').

Dataset Source: https://www.football-data.co.uk/germanym.php

Kept variables:
- FTHG = Full time Home Goals
- FTAG = Full time Away Goals
- FTR = Full time result
- HTHG = Half time Home Goals
- HTAG = Half time Away Goals
- HTR = Half time result
- HS = Shots by the home team
- AS = Shots by the away team
- HST = Shots on target by the home team
- AST = Shots on target by the away team
- Source: https://www.football-data.co.uk/notes.txt


## Summary of Findings

- Most of the Bundesliga matches were won by the Home Team.
- Most time the half time result is a draw, followed by a leading home team and away team.
- There is one match were the home team won without a single shot on target.
- The half Time Result lets us guess about the full time result.
- Percentage of wins by the home team with 3 scored goals:  87.5 %.
- If the away team does not score any goal, the number of home wins is very high.
- There is a positive correlation between the shots on target and the scored goals.
- If the Home team has more shots on target, the average win rate of the away team is around 14%.
- If the home team wins, the mean shot difference is above 2.4.
- If the result is a draw, the mean shot differnce ist between 0 and 1.
- If the away team wins, the mean shot difference is below -1.

I am going to include the most noteable findings in my explanatory analysis. First I am giving an overview of the distribution of the matches. Then I present different findings which have a bigger impact on the full time result (Shots on Target, Shot difference, Half Time Result).


## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.
- I changed the description of the axes labels to a more understandable words and did not keep the short cuts. Moreover, the size of the titles of the visualizations are made bigger to get a better view of the acutal content of the visualization.