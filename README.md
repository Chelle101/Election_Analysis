# Election_Analysis
## Election Overview
To eveluate the results of the recent local congressional election in Colorado, we are to provide an audit and detailed analysis in Python script that will be able to give the below information in regards to the election.

- Calculate the total number of votes each candidate received.
- Calculate the percentage of votes each candidate won.
- Calculate the total number of votes cast.
- Determine the winner of the election based on popular vote.
- Get a complete list of candidates who received votes.
## Election Summary

There were a total of 369,711 votes cast in the election.
### Election candidates:
- Raymon Anthony Doane
- Charles Casper Stockham
- Diana DeGette
### Results per candidate:
- Raymon Anthony Doane received 3.1% of the vote and 11,606 votes.
- Charles Casper Stockham received 23.0% of the vote and 85,213 votes.
- Diana DeGette received 73.8% of the vote and 272,892 votes.
### Winner of the election:
- Diana DeGette, who received 73.8% of the vote and 272,892 votes.

![Candidate_Results](https://user-images.githubusercontent.com/99842026/159193486-adcbfdb8-346a-4362-95c9-a423e3babd74.png)
### County Results
- The county with the largest turnout was Denver.
- Jefferson county received 10.5% of the votes and 38,855 total votes.
- Denver county received 82.8% of the votes and 306,055 total votes.
- Arapahoe county received 6.7% of the votes and 24,801 total votes.

## Evaluation of election audits
### Election aduit results
![Election_results](https://user-images.githubusercontent.com/99842026/159192379-76b4d702-4863-4c1f-9c41-c4136471c05e.png)

## Election Audit Summary
The election commission explores how this script can be used for any election, with two examples for modifying the script. If we decomposed the ask by making the following assumptions:

- We may or may not assume that every csv file will have three columns with County name and Candidate name as the second and third columns respectively.
- Users of the script may or may not have knowledge of python and they would require an easy way to specify their csv file without needing to change the file name or file path in the code.

## The Solution

We may propose a solution that provides the user with the ability to input the name of their csv file and the parent folder of the file. We would then use an indirect path method to locate and read the file on the users machine. This way our script is flexible enough to take any csv file without making any changes to the code.
Another soultion is the assumption that column names and position will not always be same for all csv files across all preccincts, we may modify our code to allow the user input the column name that contains county name and candidate name. Our script will then attempt to match user input with the column names in the csv file. Given theses implementations of two modifications, the current script can be used for any county across the US.
