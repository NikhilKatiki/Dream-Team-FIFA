# Dream-Team-FIFA
  1. Introduction
  2. Objective 
  3. Data Dictionary
  4. Data Pre-processing
  5. Feature Engineering 
  6. Sentiment Score Calculation
  8. Results
  9. Tableau Dashboard 
  10. Limitations of Score
# Introduction 
  1.Algorithms have become most integral part of working with large datasets as the computational power is very limited <br>
  2.Also, the graphs data structures has a lot of applications with increase in large datasets  <br>
  3.A lot of applications of Graph algorithms are being used by Facebook, Netflix etc., <br>
  4.Particularly, Finding a dream team requires us to know the connectedness of players <br>
  5.To find out the dream team, Linear programming is used find the best possible combination <br>
# Objective 
  1.Graph algorithms are being used to conclude about the players' network in the sports. In this case, it is Football<br>
  2.Also, the potential of the player is being predicted using few independent variables  <br> 
  3.Finally, An application of Linear Programming is used to find the best possible team with the given constraints <br>
# Data Understanding
  1.The dataset consists of 122K rows (last 5 years data) with 108 attributes of the player <br>
  2.The dataset contains the following information. Displaying the first 5 rows of the data <br>
  <img width="601" alt="Head_Players" src="https://user-images.githubusercontent.com/89437135/147394939-5a120718-d59e-4710-a1ae-511ef21bedc2.png">   <br>
  3.The potential of the player is used to understand the overall potential of the player <br>
  4.For forming the connectedness of players, either of the below two conditions need to be satisfied in order for the two players to form an edge in the graph <br>
  &nbsp;&nbsp;&nbsp;&nbsp; a.Two players are in the same club  <br>
  &nbsp;&nbsp;&nbsp;&nbsp;b. They were in the same national team in the same year<br>
# Graph Algorithms
   1. Inorder to find the connectedness of the player, Breadth for search is run to find the distance between the root vertex player and all the other connected players<br>
   2. To find the diverse set of networks in the data, Number of connected components algorithm is run
# Machine Learning  
# Data Preprocessing  
  1. Dropping the entire columns for which the missing values are greater than 10%
  2. Dropping the entire rows for which few columns are missing 
  3. Splitting the data into train and test 
# K Means Algorithm 
  1. This Model is used to understand similarity between the players based on various attributes 
# Linear Regression
  1. Linear Regression is used to predict the potential of any player given other attributes of the player 
# Decision Tree Regressor 
  1. Decision Tree is one of those which can predict the continuous variable
# Random Forest Regressor 

# Support Vector Machine 

# Linear Programming 
### Introduction
  1. Linear programming has one of the best applications in sports analytics as it is important to get all the players subject to few constraints
  2. Linear programming not only allows us to get the best players but also helps us to make decisions objectively without any inherent bias 
### Objective 
  1. The Objective of using linear programming is to find the dream team of a league based on the potential of the player with the given money and other constraints
### Data Used
  1. In this project, the league that is being used is about “Spain Primera Division” where there are 20 clubs and 645 individual players 
  2. In the preprocessing data, the labels of clubs are being converted into numeric formats to use them further 
  3. The variables considered for constraining the objective function are
      a.Goalkeeping handling
      b.Defending sliding tackle
      c.Skill dribbling
      d.Attacking volleys
      e.Potential 
Linear Programming Methodology
  1.	Creating Variables 
      a.	For every row, there is a corresponding key that is created
      b.	The key is created as binary variable 
  2.	Objective Function
      a.	The objective function consists of product key (which is defined in step 1) and players’ corresponding potential
      b.	The objective is to maximize the function described above
  3.	Constraints 
      a.	Team total purse
            i.	There would only be limited purse available to set up the team 
            ii.	This step involves the multiplication of each players’ worth with the players’ key
            iii.	The generated equation should not exceed the expected budget
      b.	One Goalkeeper
            i.	A team must have a goalkeeper 
            ii.	A good goalkeeper is someone whose goalkeeping skills are more than 50 and rest other variables values are less 
      c.	Three Mid Field players
            i.	A team must have at least three forward players 
            ii.	A good mid field player must have dribbling skills of more than 50 whereas other variables’ values can be less than 50 
      d.	Three Defensive players
            i.	A team must have three defensive players 
            ii.	A good defensive players must have defending sliding tackle skills of more than 50 whereas other variables’ values can be less than 50
      e.	Three Attacking players
            i.	A team must have three attacking players
            ii.	A good attacking player must have attacking volleys more than 50 and dribbling more than 20 
      f.	Total number of players in team 
            i.	The total team comprises 12 players 
  4.	Maximize the above defined objective function subject to constraints in step 3
### Insights
•	If the purse value of the club is “84000000” then the maximum possible total potential of team of 12 players is 1021
•	The following is the list of players which can be a dream team as per our objective function 

# Results 
  1.From the analysis, it is clear that Airbnb implemented strategies which makes them unique in responding to the pandemic <br>
  2.Sentiment dropped after March 2020, but as the company takes remedial steps, sentiment increased over time <br>
  3.Top positive and negative comments did not change much in pre and post Covid  <br>
  4.Dirty and Crowded are highlighted negative comments post-Covid which can be suggestion to Airbnb hotels which are having low sentiment scores <br>


  
