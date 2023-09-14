# Estimating the Number of Active GitHub Users Using Random Sampling

Yash Patel
Big Data Analytics, Worcester Polytechnic Institute, yppatel@wpi.edu

## 1 Introduction
The number of active github users is very large and counting them by normal means is impractical because of the time and resources it takes. To be able to solve this, we can use a sampling methodology to be able to estimate the number of active github users. With my proposed sampling method of using bins, I can say with 95% confidence that the true number of active users is between 119931537 and 120202479. 
## 2 Proposal
Estimating the total number of active GitHub users is a challenge because there are over 100 million valid GitHub ids and checking each id on whether it is valid or not can take a ton of time. Not only does it take time to extract ids from the GitHub API, but you can also only receive a maximum of 100 users per request and there is a limit on the number of requests to be made. With these limitations, a sampling method is needed to estimate the total number of active GitHub users.
	The estimation method I propose is to get the average number of active users in a set range. Then multiply the average by the number of total sets to get the estimation for the total number of active GitHub users
