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
   <br>
  3.Only the reviews column is used to find the sentiment of the customer <br>
# Data Preprocessing  
   The reviews data is in string format which needs to be converted to numeric format to find the quantitative sentiment score. Following are the steps <br> 
     1.Tokenization <br>
      &nbsp;&nbsp;&nbsp;&nbsp;    i.The sentences are being tokenized into words<br>
     2.Stemming<br>
       &nbsp;&nbsp;&nbsp;&nbsp;   i.Affixes or Prefixes are removed to reduce the dimensionality and get the words to its base form <br>
     3.Stop words<br>
       &nbsp;&nbsp;&nbsp;&nbsp;   i.Stop words which are frequently used are being removed as these dont contribute to the overall sentiment of the customer <br>
     4.Numeric formats <br>
        &nbsp;&nbsp;&nbsp;&nbsp;  i.Numeric formats have been removed as these are not useful in understanding the review <br>
# Feature Engineering 
   Positive words and Negative words <br>
         &nbsp;&nbsp;&nbsp;&nbsp; i.Finding the number of positive words and negative words for every review <br>
          &nbsp;&nbsp;&nbsp;&nbsp;ii.Storing number of positive words in positive and number of negative words in negative <br>
# Sentiment Score Calculation 
   The score is calculated using the formula: <br>
          Sentiment score = (#Positive)/(#Positive+#Negative) when #Positive>#Negative <br>
                        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  =-(#Negative)/(#Positive+#Negative) when #Positive>#Negative<br>
                        <img width="600" alt="Sentimentscore" src="https://user-images.githubusercontent.com/89437135/147394661-cdb53265-33ad-4630-8bd2-ffe5524f7b81.png">
<br>
# Results 
  1.From the analysis, it is clear that Airbnb implemented strategies which makes them unique in responding to the pandemic <br>
  2.Sentiment dropped after March 2020, but as the company takes remedial steps, sentiment increased over time <br>
  3.Top positive and negative comments did not change much in pre and post Covid  <br>
  4.Dirty and Crowded are highlighted negative comments post-Covid which can be suggestion to Airbnb hotels which are having low sentiment scores <br>
# Tableau Dashboard 
https://public.tableau.com/app/profile/katiki.nikhil

  
# Limitations of Score 
    1.The list of positive words and negative words is limited to the one which is provided as input 
    2.There are equal weights assigned to each and every word 
    3.The Analysis wont capture the phrases such as "not good". This sentence has neutral score whereas it is to be tagged as negative 
  
