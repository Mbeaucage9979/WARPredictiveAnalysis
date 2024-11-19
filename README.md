# WARPredictiveAnalysis
Predicts the WAR (Wins Above Replacement) for Professional Baseball Players using trend analysis
This project uses Python and the 'pybaseball' feature to analyze player performance from past seasons, as well as predict player performance for upcoming seasons.
The initial code uses the 2015 - 2023 seasons to predict the 2024 season, so accuracy could be tested and examined with already available data. Changing the years is not difficult, as soon as data becomes available in pybaseball.
** Step 1 **
Fetch player data (WAR, OBP, SLG, HR) for a range of years using pybaseball
** Step 2 **
Organize data insto a single dataset
Generate features ('WAR_Last_Year', 'WAR_2_Years_Ago', etc..) for predictive modeling
** Step 3 **
Train a Random Forest refression model to predict WAR for future season/seasons.
Evaluate the model using RMSE and R2.
** Step 4 **
Predict the War

Example Output:
RMSE: .913
R2 Score: 0.75

Top 10 Players by Predicted WAR
1. Player 1        8.500
2. Player 2        7.978
3. Player 3        7.320

*** NOTE ***
You bust install 'pybaseball' by running the following first

#!pip install pybaseball
#import pybaseball


** Known Areas of Improvement ** 
Currently, the code requries a minimum of 100 plate appearances for players to be considered in the pedictions. I am aware of the fact that this unfairly filters out pitchers.
