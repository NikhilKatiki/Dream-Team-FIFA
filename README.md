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
## K Means Algorithm 
   This Model is used to understand similarity between the players based on various attributes <br>
 
 <img width="572" alt="01" src="https://user-images.githubusercontent.com/89437135/150624091-b7ac5f65-0300-44f5-8261-dae3ca07f68f.png">;

## Linear Regression

<img width="567" alt="02" src="https://user-images.githubusercontent.com/89437135/150624098-1459d138-4b72-4609-b080-a5f3641ac8db.png">;
## Decision Tree Regressor 
 
 <img width="574" alt="03" src="https://user-images.githubusercontent.com/89437135/150624103-373e8011-cf08-4460-95e8-2bcd6dea6784.png">;
## Random Forest Regressor 
<img width="575" alt="04" src="https://user-images.githubusercontent.com/89437135/150624105-f6d3f32c-65da-4035-aad5-55b8c90b374f.png">;

## Support Vector Machine 

<img width="569" alt="05" src="https://user-images.githubusercontent.com/89437135/150624110-54cdb90d-31b2-4fdc-92aa-79d8dc95ba35.png">;
# Linear Programming 
## Introduction
  1. Linear programming has one of the best applications in sports analytics as it is important to get all the players subject to few constraints <br>
  2. Linear programming not only allows us to get the best players but also helps us to make decisions objectively without any inherent bias <br>
## Objective 
  1. The Objective of using linear programming is to find the dream team of a league based on the potential of the player with the given money and other constraints<br>
## Data Used
  1. In this project, the league that is being used is about “Spain Primera Division” where there are 20 clubs and 645 individual players <br>
  2. In the preprocessing data, the labels of clubs are being converted into numeric formats to use them further <br>
  3. The variables considered for constraining the objective function are<br>
      a.Goalkeeping handling<br>
      b.Defending sliding tackle<br>
      c.Skill dribbling<br>
      d.Attacking volleys<br>
      e.Potential <br>
Linear Programming Methodology<br>
  1.	Creating Variables <br>
      a.	For every row, there is a corresponding key that is created<br>
      b.	The key is created as binary variable <br>
  2.	Objective Function<br>
      a.	The objective function consists of product key (which is defined in step 1) and players’ corresponding potential<br>
      b.	The objective is to maximize the function described above<br>
  3.	Constraints <br>
      a.	Team total purse<br>
            i.	There would only be limited purse available to set up the team <br>
            ii.	This step involves the multiplication of each players’ worth with the players’ key <br>
            iii.	The generated equation should not exceed the expected budget<br>
      b.	One Goalkeeper<br>
            i.	A team must have a goalkeeper <br>
            ii.	A good goalkeeper is someone whose goalkeeping skills are more than 50 and rest other variables values are less <br>
      c.	Three Mid Field players<br>
            i.	A team must have at least three forward players <br>
            ii.	A good mid field player must have dribbling skills of more than 50 whereas other variables’ values can be less than 50 <br>
      d.	Three Defensive players<br>
            i.	A team must have three defensive players <br>
            ii.	A good defensive players must have defending sliding tackle skills of more than 50 whereas other variables’ values can be less than 50<br>
      e.	Three Attacking players<br>
            i.	A team must have three attacking players<br>
            ii.	A good attacking player must have attacking volleys more than 50 and dribbling more than 20 <br>
      f.	Total number of players in team <br>
            i.	The total team comprises 12 players <br>
  4.	Maximize the above defined objective function subject to constraints in step 3<br>
### Insights
•	If the purse value of the club is “84000000” then the maximum possible total potential of team of 12 players is 1021
•	The following is the list of players which can be a dream team as per our objective function 
<img width="497" alt="06" src="https://user-images.githubusercontent.com/89437135/150624116-6a8ca48f-3eb0-4dd3-9365-107656068a01.png">

# Results 
  1. Graph Structures are very helpful in Network analysis 
  2. Optimization particularly in sports plays a major role in finding the best combinations with the specified constraints 

# Thank You!

  
