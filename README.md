# Machine-Learns-Sports-Betting

## Using several Machine Learning alogorthims, will we able to find a model that will help us beat vegas?
### Can the model predict which team would be the winner?
### Can the model predict whether the team is the loser or winner based on win spread?

### Data Gathering / Cleaning 
* Using pandas we were able to gather data from serveral websites and had to clean the data.
* Cleaning the data meant changing any game in which we had a tie, to a loss.
* Fill in missing information that was lost when scraping. 
* We had to merge several tables in order to get all the informations into one this includes, team power rankings, yards, turnovers, etc...
* Calculate net yards, turnovers, points, for every team prior to the game they were going to play. 
  - For example in week 1 of game every team had 0 in every field but if team A scored 21 points, with 300 yards, and 2 turnovers in week 1's game, you would see this for week 2's game they are going into. 
  
### Logistic Regression 
- For the win, using logistic regression we were able to get a accuracy of 67% for the test set, which was suprisingly higher than our training set which got a accuracy of 65%. 
- For the win spread, we were able to get a accuracy of 51.1%

### Deep Nueral Network 
- For the win, using a Deeo Nueral Network we were able to get a accuracy of 67% again.
- For the win spread, we were able to get a accuracy of 53.3% 

### Random Forest (Best Model)
- For the win, the accuracy was a constant 70% after using grid search to find the optimal parameters. 
  - The features that had the highest impact turned out to be spread and the teams net yards
  For the win spread, the highest accuracy we got was 54%. 
  
### Results
#### With our best model we were able to achieve a accuracy of 70% in predicting the winner and 54% for the win spread. The 54% does not seem impressive at first but By using an expected outcome formula, we find that being able to correctly pick the spread at >52% means you can  “beat the odds” on your typical -110 bet and win money. Thus our 54% is actually pretty good!!! After calculations we were able to calculate that for every bet you would have a return of $4.24 or 4% 

# [Link to presentation:](https://github.com/MGao535/Machine-Learns-Sports-Betting/blob/master/Final/Beating%20Vegas%20using%20Machine%20Learning%20.pdf)

![Image of Graph](https://user-images.githubusercontent.com/35829105/93822462-e2f64000-fc25-11ea-994a-565302371c72.png)
