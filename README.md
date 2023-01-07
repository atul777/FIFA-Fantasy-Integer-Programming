# FIFA-Fantasy-Integer-Programming
Fantasy leagues are catching up heat in the recent years. Most fans use their intuition while assembling their fantasy teams because there is no perfect mantra to win. It is also highly dependent on your luck as fine margins decide who wins these leagues. But what if we ask optimization experts with no knowledge of the game to place a team, they see this as a binary integer problem. To help the fans to assemble the perfect FIFA World Cup Fantasy team, our team is building a binary integer optimization model very much like the capital budgeting program we did in class. Our model is a data-driven approach to consider the historical data to create an optimal list of players for your fantasy team.
To summarize, our model tries to maximize the overall points of 11-starting players (plus 4 substitutions) with a 100-million-dollar budget. Each player cost varies price but with different scoring potential, which will be quantified with our predicting model. There are several constraints taken into consideration:
1.	Total players Constraint: The primary hard constraint that we have is that our fantasy team can only comprise 15 players.  
2.	Budget Constraint: There is a budget cap of $100 million and each player has a price tag
3.	Position Constraints: You are allowed to have at max 3 forwards, 5 midfielders, and defensive players. There will be at least one goalkeeper as well in the team. These are all the possible formations that a playing 11 can have:   
 4-4-2
 4-3-3
 4-5-1
 3-4-3
 3-5-2
 5-2-3
 5-3-2
 5-4-1 

Apart from this, we also need to choose our 4 substitutes, one of which must be a goalkeeper. Although points from these players do not contribute to our fantasy points, these players have a price tag and must follow the total budget constraint.
4.	National Team Constraint: You are allowed to choose 5 players max per nation for the quarterfinals.
5.	Yellow Card Constraint: A player who got 2 yellow cards in consecutive games can’t play the next game  
6.	Red Card Constraint: A player who gets a red card cannot play the next game.
