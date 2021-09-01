# Cash-Flow-Minimizer
The idea is to use Greedy algorithm where at every step where we settle all amounts of one person and recur for remaining n-1 persons. 
# Algorithm
1. For every person Pi, from 0 to n – 1, do the following steps
2. Compute the net amount for every person. Net mount for a person I can be computed by subtracting the sum of all debts from the sum of all credits.
3. Find maximum creditor Pc and maximum debtor Pd. Suppose the maximum amount to be credited to a maximum creditor is max_credit, and the maximum amount debited from a maximum debtor is called max_debit.
4. Set x: = minimum of max_credit and max_debit. Then debit x from Pd, and credit x to Pc
5. If x is the same as the max_credit, then remove Pc from the set and recur for next n-1 persons.
6. If x is same as max_debit, then remove Pd from a set of persons and recur for next n-1 persons.
