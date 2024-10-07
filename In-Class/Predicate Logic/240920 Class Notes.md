## Warm Up

Prove that there exists an integer n such that n > 100

Proof:
Proof by example.
Assume `n` = 200
`n` > 100 holds
There exists an integer n such that n > 100. ∎

## Proof By Example
If we can show that there is a value of x that x > 20

Set y = x. That shows that there is a value of y > 20, which means there also is a value of x > 20

## Multiple Quantifiers in a Statement

∀ m ∈ Z, ∃ n ∈ Z such that n > m.

For all integer numbers, there exists a larger integer.

Proof:
Let `m` be an arbitrary integer
Proof by example.
Set `n` = `m` + 1
Then the statement becomes `m + 1` > `m`, which is true.
This completes the proof. ∎



## Practice

∃ m ∈ Z, such that ∀ n ∈ Z, n > m

There exists an integer m such that all integers n are greater than m

This argument is invalid


Try and negate the statement above:
¬(∃ m ∈ Z, such that ∀ n ∈ Z, n > m)
Becomes
∀ m ∈ Z, ¬(∀ n ∈ Z, n > m)
Becomes
∀ m ∈ Z, ∃ n ∈ Z s.t. n ≤ m

Which intuitively is 
For all integers, there is an integer less than it.

You could then prove the negation, thereby proving the original argument invalid