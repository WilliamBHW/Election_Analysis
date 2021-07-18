# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the toal number of votes cast.
2. Get a complete list of candidates who recieved votes.
3. Calculate the total number of votes each candidate recieved.
4. calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.
6. Calculate voter turnout for each county.
7. Calculate the percentages of votes from each county.
8. Determine the largest county based on turnout.

## Resourcces
- Data Source: election_results.csv
- Software: Python 3.8.2, Visual Studio Code 1.58.2

### Challenge Data Background
> After giving you an overview of the election audit tasks, Tom wants to go over the steps required in detail. He's going to show you a technique commonly used by programmers to write steps of their code, which is called pseudocode. Pseudocode will make the audit easier to present to nontechnical colleagues and stakeholders.

To facilitate the design process, programmers use pseudocode to create models or flowcharts for their programs. Pseudocode is like a roadmap of what you think your code will look like or the steps you'll take to complete the task at hand.

Pseudo means "fake," so pseudocode is essentially fake code. Pseudocode is an informal language that has no syntax rules and is not meant to be executed. The point of using pseudocode is to focus on the overall design of the program.

## Election-Audit Results
The analysis of election show that:
- There were 369,711 votes cast in the election
- The counties were:
  - Jefferson
  - Denver
  - Arapahoe
- The county result were:
  - Jefferson recieved 10.5% of the turnout and 38,855 number of turnouts.
  - Denver recieved 82.8% of the turnout and 306,055 number of turnouts.
  - Arapahoe recieved 6.7% of the turnout and 24,801 number of turnouts.
- The county with largest turnout was:
  - Denver , which recieved 82.8% of the turnout and 306,055 number of turnouts.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham recieved 23.0% of vote and 85,213 number of votes.
  - Diana DeGette recieved 73.8% of vote and 272,892 number of votes.
  - Raymon Anthony Doane recieved 3.1% of vote and 11,606 number of votes.
- The winner of the election was:
  - Diana DeGette , who recieved 73.8% of vote and 272,892 number of votes.

## Election-Audit Summary
The source folder and code are in the same location so that it is easy to read files from sources and make manipulations. Destination folder ("analysis") can be created in the same location which will compose destination files in assigned folder. This script uses universal/global variables to take record of elections data such as `candidate_options`, `county_options`, `candidate_votes`, `county_votes` etc. In the script, these variables are commonly used in the following criterias:
- Record candidate names & county names
- Record total votes
- Record candidate votes & county turnout
- Record realative winning candidate & county
- Record relative percentages

#### Global Variables
![files to save/load](https://github.com/WilliamBHW/Election_Analysis/blob/main/Resources/file_to_change.png)
![global](https://github.com/WilliamBHW/Election_Analysis/blob/main/Resources/county_setup.png)
<br>
These global variables can be refered to different locations by simply changing its pointer. These variables are being used here to take any data from calculations or assignments. Final values and result usually being stored in these global variables for future reference.
<br>

Local variables are used in for loop and conditional statements such that they are calculating data that will be saved into global variables. (ex. `candidate_name`, `county_name`, `cvote`, `cvote_percent`)
#### Local Variables
![calculation](https://github.com/WilliamBHW/Election_Analysis/blob/main/Resources/county_main.png)
![messages](https://github.com/WilliamBHW/Election_Analysis/blob/main/Resources/modify.png)
<br>
These local variables inside functions are responsed for making calculations and record result of calculation, they are flexible with any calculation and assignment. For instance, `cvote_percent` is being assigned a formula which could be modified anyway user want it to be. Messages are written to txt file with the reference of global variables that were assigned local values.
<br>

Overall coding structure is consist of persudo code, functions, global variable and local variable. With persudo code outline main functionalities of the project, we are able to use the rest to form chunks of the script and after all, complete full script to compose data summarization.
