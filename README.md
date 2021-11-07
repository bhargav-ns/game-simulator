# game-simulator
A Blackjack simulator to demonstrate key concepts in statistics and simulation strategy

After extraction, two executable python scripts will be available: one in .ipynb format and another in .py format.

Running the .ipynb file is ideal, since it is easier to visualize the outputs. The seaborn package may also not work with the .py file.

Python version : 3.7.9
Required Packages : Latest versions of Numpy, Seaborn, Scipy, Matplotlib, and Pandas

The code contains 4 main functions:
- PlayerGuide: This is an attempt to emulate optimal Blackjack strategy. It contains the decisions that will be made by 
the player over the course of a single run. The initial cards for the dealer and the player can be set while calling the
function. 

- blackjack_round: Simulates a single round of blackjack with simple conditional statements. 
The bet amount, payback type, initial conditions, and dealer's 'stay' threshold can be passed while calling the function.

- blackjack_sim: Simulates 'n' blackjack rounds. Returns a tuple containing the initial conditions, number of runs, and
list of payouts aggregated over all the rounds.

- compute_stats: Takes the output of blackjack_sim as the input and outputs variance, confidence intervals for the mean,
kernel density plots for distribution of payouts, and so on.


Open the .ipynb file in a Jupyter Notebook and run all the cells. Alternatively, just run python blackjack.py in the terminal 
after installing the required packages.
