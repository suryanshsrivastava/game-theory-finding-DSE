## Language and modules
*Language:* python3
*Modules imported:*
* sys
* numpy
* itertools

##Displays all dominant strategy equilibria for a n-player game

To run the file
DSE.py <inputfile> <outputfile>

sample command:
assignv3.py Example1.nfg out.txt

## Input Format 

If file is not provided it will throw error "Please pass the name of the game file to be analyzed"

Input file should be in NFG format
line 1:		Static Content with Title
line 2:		{ Space seperated, double quoted player names } { space seperated integers of #strategies in respect to the players }
line 3:
line 4:		space seperated integers of payoffs to all players for each stratgies combination.


line 1:		NFG 1 R "Example1"
line 2:		{ "Player 1" "Player 2" } { 3 3 }
line 3:
line 4:		2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 3 3

## Solution approach
The approach uses brute-force method. It iterates over each player one by one.
In the i<sup>th</sup> iteration it finds the best action s<sub>i</sub> for all possible values of the strategy S<sub>-i</sub> of all other players. If the interesction of s<sub>i</sub> for all possible S<sub>-i</sub> is null for any player then no dominant strategy equilibrium exists else atleast one exists.

## Time Complexity
The complexity is O(N * A).
where N is the number of players
and A is the product of the number of actions available to each player
