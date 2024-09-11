## Warm Up
Prove:
```
p → q
q → r
∴ p → r
```
If `p` is false then `p → r` is always true, so we only need to consider if `r` is true when `p` is true.
In that case, if `p` is true then `q` must also be true by Modus Ponens
If `q` holds, then `r` also holds by Modus Ponens

Then, if `p` is false then `p → r` is true, and if `p` is true, then that makes `r` true, which means `p → r` is also true then.

This argument is used as a **Rule of Inference**. It is known as the Transitivity Rule. It works like a chain, where each one implies the next.

## Proof of P → R
Idea:
Assume that p holds, and using that assumption, prove that r holds

Formal Proof Of:
```
p → q
q → r
∴ p → r
```
Assume `p` holds Temporary Assumption
Since `p` holds, and `p → q`, `q` also holds. (Modus Ponens)
Since `q` holds, and `q → r`, `r` also holds. (Modus Ponens)
We have shown that `p → r` ∎

## Temporary Assumption
This is an Assumption we make in our proof that lasts for a certain few lines until we take a step back. 
In the example above, the Temporary Assumption of `p` lasts until the end of the second since

## Proof By Contradiction
### Main Idea
Assume the negation of what we want to prove, then arrive at a contradiction
### Real Example

If n^2 = 100
n ≠ 4

We can prove this by saying "Well if n was four, n^2 would be 16, which is not 100"

### Example
```
p → ¬q
p → ¬r
q ∨ r
∴ ¬p
```

Assume for contradiction that `p` holds 
	Since `p` holds and `p → ¬q`, `¬q` holds
	Since `¬q` holds and `q ∨ r` holds, `r` must hold
	The fact that `p` holds and `r` holds, makes `p → ¬r` a contradiction
We have shown by contradiction that `p` must be false. ∎

## Examples / Practice

### Example 1
```
p → s
(q ∧ s) → r
∴ (p ∧ q) → r
```

Assume `(p ∧ q)` holds                                                                (Temporary Assumption)
Since `(p ∧ q)` holds, `p` holds and `q` holds                             (∧-Elimination)
Since `p` holds and `p → s`holds, `s` also holds                          (Modus Ponens)
Since `q` holds and `s` holds, `q ∧ s` holds                                  (∧-Introduction)
Since `q ∧ s` holds and `(q ∧ s) → r` holds, `r` also holds    (Modus Ponens)
We have shown that `(p ∧ q) → r`  ∎

### Practice 1
```
p → q
p → ¬r
∴ p → (q ∧ ¬r)
```

Assume `p` holds                                                                                 (Temporary Assumption)
	Since `p` holds and `p → q` holds, `q` must also hold           (Modus Ponens)
	Since `p` holds and `p → ¬r` holds, `¬r` must also hold       (Modus Ponens)
	Since `¬r` holds and `q` holds, `q ∧ ¬r` also holds               (∧-Introduction)
We have shown that `p → (q ∧ ¬r)`  ∎

### Practice 2
```
q → (p ∧ r)
p → ¬r
∴ ¬q
```

Assume `q` holds                                                                                                     (Temporary Assumption)
	Since `q` holds and `q → (p ∧ r)` holds, `p ∧ r` holds                           (Modus Ponens)
	Since `p ∧ r` holds, both `p` and `r` hold individually                               (∧-Elimination)
	The fact that `p` holds and `r` holds makes `p → ¬r` a contradiction.   (Contradiction)
We have shown that `q` must be false. ∎