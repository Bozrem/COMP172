### If and Only If
Ex: n is an even integer if and only if n+1 is an odd integer
Symbol: ↔ (left right arrow in unicode)

Can be built as two if statements connected by an "and"

Expanded example:
(if n+1 is an odd integer then n is an even integer) and (if n is an even integer, then n+1 is an odd integer)

Symbol notation:
n ↔ p
can also be
(n → p) ∧ (p → n)

"n is even only if n+1 is odd" 
Is saying the same thing as
"if n is even, then n+1 is odd"

## Argument
#### Example 1
Hypothesis: If my code is correct, then it passes my unit tests
Hypothesis: My code passes my unit tests
Conclusion: My code is correct

This argument is not valid because the nature of the conditional means that assuming it is true has scenarios where it isn't true.

### Definitions
Hypothesis/Premise: A logical statement that we assume/assert is true
Critical Row: A row in the Truth Table where all hypothesis are true

### Notes
To refute an argument:
* Refute a hypothesis being true
* Refute the logic working (Like example 1)

An argument is ***valid*** if the conclusion follows from the hypotheses/premises.
An argument is ***sound*** if it is valid and the hypotheses are true

### Determining Argument Validity
Using Example 1:
c = "my code is correct"
t = "my code passes my unit tests"

First hypothesis: c→t
Second hypothesis: t
Conclusion: c

Notated:
```
c→t
t
∴c
```

To determine the validity of this argument:

1. Make a truth table with a column for each hypothesis and conclusion
2. Identify the ***Critical Rows*** (each row where all hypotheses are true)
3. If the conclusion is true in every critical row, then the argument is valid
	1. If the conclusion is false in any critical row, then the argument is invalid

| c     | t     |     | c→t   | t     | c     |
| ----- | ----- | --- | ----- | ----- | ----- |
| 0     | 0     |     | 1     | 0     | 0     |
| ==0== | ==1== |     | ==1== | ==1== | ==0== |
| 1     | 0     |     | 0     | 0     | 1     |
| ==1==     | ==1==     |     | ==1==     | ==1==     | ==1==     |
From the truth table constructed, we can see that the critical row with c = 0 and t = 1 does not support the conclusion, so the argument is invalid.

## Practice
### Is This Argument Valid?
```
p → r
p
¬q → ¬p
∴ r ∧ p
```


| p     | q     | r     |     | q → r | ¬q → ¬p |     | r ∧ p |
| ----- | ----- | ----- | --- | ----- | ------- | --- | ----- |
| 0     | 0     | 0     |     | 1     | 1       |     | 0     |
| 0     | 0     | 1     |     | 1     | 0       |     | 0     |
| 0     | 1     | 0     |     | 0     | 1       |     | 0     |
| 0     | 1     | 1     |     | 1     | 1       |     | 1     |
| 1     | 0     | 0     |     | 1     | 0       |     | 0     |
| 1     | 0     | 1     |     | 1     | 0       |     | 0     |
| 1     | 1     | 0     |     | 0     | 1       |     | 0     |
| ==1== | ==1== | ==1== |     | ==1== | ==1==   |     | ==1== |
The argument only has one critical row of {p, q, r} = {1, 1, 1}, in which the conclusion r ∧ p is true. Therefore, since all critical rows are true, the argument is valid.

### Is This Argument Valid
```
p → q
q → p
∴ p
```


| p     | q     |     | p → q | q → p | p     |
| ----- | ----- | --- | ----- | ----- | ----- |
| ==0== | ==0== |     | ==1== | ==1== | ==0== |
| 0     | 1     |     | 1     | 0     | 0     |
| 1     | 0     |     | 0     | 1     | 1     |
| ==1== | ==1== |     | ==1== | ==1== | ==1== |
The argument is invalid because it has critical row p = 0, q = 0 in which the conclusion p is false.
