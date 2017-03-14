## Determining the optimal number of upsets

This is code I wrote for the analysis in this article

https://www.wsj.com/articles/stop-picking-so-many-ncaa-tournament-upsets-1489429650

The question the article is trying to answer is how many upsets you should pick based on how big of a pool you are in.

A quick summary of the method, this was simulated 1000 times for each (group size, tournament) combination since 2000. 

	- Create a group of size n, with each player in the group having a different "risk factor" between 0 and 1
	- For each player simulate them picking a bracket, with the bernoulli probability of them picking an upset in each game equal to their "risk factor" divided by the strength of an upset (so someone doesn't pick 16 over 1 with the same frequency as 4 over 2)
	- Take the average number of upsets picked (both total and for each round) for the winners in every group size, average across all tournament years





