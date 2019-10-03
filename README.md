# Predicting NBA player salaries

### Project Goal:
The goal here is to build a model that can help team manager to see whether their salary spending is worthy it or not. And for player, this model can help them understand what are the features they need to improve on in order to get more salaries. 
Building a linear regression model is the most suitable approach in this case since all of the players'performance statistics are measured in continuous numbers. In order to prevent model overfitting the training data too much, I use r square and RMSE as metrics to compare different models and choose the one that gives me the lowest RMSE. From then, if the r square value is too low, I will transform the data using reguarlization to prevent overfitting. 
Note: NBA Salary Cap is the limit to the total amount of money that National Basketball Association teams are allowed to pay their players. Like many professional sports leagues, the NBA use this salary cap to control fairness of the games. It varies every year based on last season's revenue. With the existence of Salary Cap, bigger and rich teams are not supposed to spend more money to recruit all of the more talented players. However, this limit is a soft cap.  A team can still sign players or make trades that exceed the cap under certain conditions. And they will need to pay more taxes as penalty. There are many other factors that can affect players' salaries, such as players'injuries and luxury cap. Therefore, this project is a partial predictive model, but it's good to see what are some factors that can affect players'salaries.


### Install

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [sklearn](https://scikit-learn.org)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)


### Run

In a terminal or command window, navigate to the top-level project directory and run one of the following commands:


```bash
Project 2 Web Scraping.ipynb
Project 2 NBA Player Salary Predictions-Final.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

#### Data:

 * Team Rating: https://www.basketball-reference.com/leagues/NBA_2019_ratings.html
 * NBA Player Salaries: http://www.espn.com/nba/salaries/_/year/2019/page/
 * Team Abbreviation: https://en.wikipedia.org/wiki/Wikipedia:WikiProject_National_Basketball_Association/National_Basketball_Association_team_abbreviations
 * Players WinShare Statistics: https://www.basketball-reference.com/play-index/psl_finder.cgi?request=1&match=single&type=advanced&per_minute_base=36&per_poss_base=100&lg_id=NBA&is_playoffs=N&year_min=2019&year_max=2019&franch_id=&season_start=1&season_end=-1&age_min=0&age_max=99&shoot_hand=&height_min=0&height_max=99&birth_country_is=Y&birth_country=&birth_state=&college_id=&draft_year=&is_active=&debut_yr_nba_start=&debut_yr_nba_end=&is_hof=&is_as=&as_comp=gt&as_val=0&award=&pos_is_g=Y&pos_is_gf=Y&pos_is_f=Y&pos_is_fg=Y&pos_is_fc=Y&pos_is_c=Y&pos_is_cf=Y&qual=&c1stat=&c1comp=&c1val=&c2stat=&c2comp=&c2val=&c3stat=&c3comp=&c3val=&c4stat=&c4comp=&c4val=&c5stat=&c5comp=&c6mult=&c6stat=&order_by=ws&order_by_asc=&offset=0
 * Players Basic Statistics: https://www.basketball-reference.com/leagues/NBA_2019_per_game.html
