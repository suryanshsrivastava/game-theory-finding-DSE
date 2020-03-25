# Game-Theory Assignment1 Question2
Assignment1: ​ Find​ ​ all dominant strategy equilibria for an n-person game given nfg file 
<!-- (The problem statement has been updated) -->

You need to write your solution approach and time complexity in the readme file.

To run the file
./run <input file> <output file>

sample command:
./run Example1.nfg output1

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

Time Complexity:
O(#players X #strategies of that players)
