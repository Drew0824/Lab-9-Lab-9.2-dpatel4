# Simplifying multiway if-else statements
This is program for a state that computes tax according to the rate schedule:
- No tax on first $15,000 of income
- 5% tax on each dollar from $15,001 to $25,000
- 10% tax on each dollar over $25,000

The program uses a multiway if-else statement with one action for each of these three cases. Run the program for each of the three cases and verify it works as you expect.

The condition for the second case is actually more complicated than it needs to be. The computer will not get to the second condition unless it has already tried the first condition and found it to be false. Thus, you know that whenever the computer tries the second condition, it will know that netIncome is greater than 15000.  

Therefore the line
`else if (( netIncome > 15000) && (netIncome < = 25000))`
can be replaced with
`else if (netIncome <= 25000)`
because it is already determined that `netIncome > 15000`

Make this replacement in the program and verify it works as expected.