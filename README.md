# nbamvppredictor
Model to predict most likely players to win MVP through stats

Current model used is linear regression as a test. Currently set to use past 10 MVP votes, though the number of past seasons can be adjusted for more or less. For each past season, script takes top 5 MVP vote getters and their points per game, rebounds per game, assists per game, Player Efficiency Rating, and Win Shares per 48, along with their vote share that season. Model uses this data as training data, training on points per game, rebounds per game, assists per game, Player Efficiency Rating, and Win Shares per 48, and using vote share as the predicted value to see how likely they are to win. 

To choose a different season to predict MVP on, change the value of the 'Season' variable to the specified year. The year selected is the second of the two for a typical season year. For example, if want 2022-23 season, set 'Season' to 2023. 

To adjust training data to add more or less past MVP voter data, adjust the first for loop to loop more or less times
