# Data Setup / Recovery
- d1 . imports
- d2 . sqllite db setup
- d3. match_detail 

# Preview Database Tables
- i1

# Number of Leagues / countries
- s1. 11
# number of teams
- s2. 299
# biggest league by team count
- s3. France Ligue 1
# smallest league by team count
- s3. Switzerland Super League
# Number of seasons
- s4. 8 seasons
# first season
- s4. 2008/2009
# last season
- s4. 2015/2016
# number of matches per season
- s5. ~3247.375
# number of matches per league per season
- s6
# did any team play in more than one league?
- s7. no
# how many players are there for the entire dataset?gg
- s8. 11060 
# Does match table refer to fifa id or api id?
- s9. non-fifa api ida, player_api_id
# For each player, find matches they played in
- s10
# Get top 10 players played that the most games
- s11 . Steve Mandanda was the most active player
# for each of the top 10 players who played the most games, get # of seasons they played, first and last
- s12
# Total players that played per season
- s13
# were there any players that traded teams that were in different leagues?
- s14, yes, 1785 players traded and played in different leagues. Gelson Fernandes played in the most different leagues in this time period

# were there any players that played all 8 seasons?
- s12 Yes
# most traded player
- s13. Sergio Floccari was the most traded player
# which players had the most goals/assists?
- s15
# which players had the most goals, per season?
- s16
# is the foulcommit data accurate?
- s17
# Which players had the most penalties
- s18
# what kinds of penalties are there, and their counts
- h3 tool
- s20 p1,p2
# which players have the most penalties per season?
- s21
# do all fouls have cards associated with them?
- s22
- no. match_id = 3656
- https://www.quora.com/What-is-the-difference-between-a-foul-in-soccer-and-a-yellow-or-red-card
# Fix match_cards since some player1  values are invalid (missing or is 'Unknown player') 
- s23 datafix
# which are the most violent players?
## Are there any matches were a player had 3 card_types in a single match?
- s24
- m_id(21846)     p_id(33586      3)
# top 10 matches with most fouls
- s25
# top 10 players with most fouls 
- s26

# for each team, what was the the number of wins per season?
- s27

## foulcommit and card columns
- m2
# What teams improved the most over the time period?
# what team attributes lead to the most victories?
# Which league has the best teams?
# average points per game
# field with best home court advantage
# verify outliers theory. what is the age of 
# is there a correlation between fouls and wins or losses?
# win rate home vs away correlation?
# best goalie?
# what is the correlation of goalie rating vs win rate or championship rate?
# how many matches have missing or probably incorrect data?
# try to graph wins or score per stage for a given team
- g1 pending



# Tools
# quick xml column reviewer 
- h1
```
col = 'cross'
quick_xml_column_reviewer(col,match_detail)
```
# view columns minified (for long column lists)
- h2
#  quick xml column parser to see value counts of xpath values in a dictionary 
- h3
# misc notes
# What is home_player_X1 / home_player_Y1 mean?
- m1
https://www.kaggle.com/hugomathien/soccer/discussion/80756

# European Soccer Database Supplementary Data
- m2
https://www.kaggle.com/jiezi2004/soccer

# explanation of alot of the columns
- m3
http://www.football-data.co.uk/notes.txt

# types of fouls and their severities
- m4
https://www.ducksters.com/sports/soccer/rules_fouls.php


# TODO 
- Organize the insights by grouping 
 - General Insights
 - League Insights
 - Cross disiplinary insights
  - ie, most traded players 
 - Team Insights
 - Player Insights
 - Season Insights
 - Insights about the game as a NOOB
    - 2 yellow cards is a red card, thats why I was unable to find a red card and 2 yellow cards for a given player
 - explain the reference tags heuristics / naming convention
   - 
 