## Question 1: Proof
Argument:
```
p
q → r
¬q → ¬p
∴ r
```

Since `¬q → ¬p` holds, `p → q` must also hold                                               (Contrapositive)
Since `p` holds and `p → q` holds, `q` must also hold                                    (Modus Ponens)
Since `q` holds and `q → r` holds, `r` must also hold                                    (Modus Ponens)
We have shown that `r` must hold ∎

## Question 2: Proof
Argument:
```
q
p ∨ r
∴ ¬r → (p ∧ q)
```

Assume `¬r` holds                                                                                               (Temporary Assumption)
	Since `¬r` holds and `p ∨ r` holds, `p` also holds                                  (∨-Elimination)
	Since `p` holds and `q` holds, `p ∧ q` holds                                            (∧-Introduction)
Assume `r` holds                                                                                                 (Temporary Assumption)
	Since `r` holds, `¬r → (p ∧ q)` also holds                                            (Modus Ponens)
We have shown that `¬r → (p ∧ q)` always holds. ∎

## Question 3: Proof
Argument:
```
p → (q ∨ r)
¬r
q → r
∴ ¬p
```

Assume `p` holds for contradiction                                                                 (Temporary Assumption)
	Since `p` holds and `p → (q ∨ r)` holds, `q ∨ r` must also hold     (Modus Ponens)
	Since `¬r` holds and `q ∨ r` holds, `q` must also hold                        (∨-Elimination)
	Since `q` holds and `q → r` holds, `r` must hold                                   (Modus Ponens)
	We have a contradiction in both `r` holding and `¬r` holding             
We have shown that `¬p` must hold by contradiction. ∎

## Question 4: Proof
Argument:
```
p ∨ q
q → r
(p ∧ s) → t
¬r
¬q → (u ∧ s)
∴ t
```

Since `¬r` and `q → r` hold, `¬q` holds                                                             (Modus Ponens)
Since `¬q` and `¬q → (u ∧ s)` hold, `u ∧ s` holds                                        (Modus Ponens)
Since `u ∧ s` holds, both `u` and `s` hold                                                        (∧-Elimination)
Since `¬q` and `p ∨ q` hold, `p` holds                                                               (∨-Elimination)
Since `p` and `s` hold, `p ∧ s` holds                                                                 (∧-Introduction)
Since `p ∧ s` and `(p ∧ s) → t` hold, `t` holds                                           (Modus Ponens)
We have shown that `t` holds. ∎

## Question 5: Proof of Python
#### Prove:
```
for all booleans b:
b == False is the same as !b

∀ b ∈ B, P(b)
P(b) = ((b == False) == !b)
```

Assume `b` is True
	`b == False` evaluates to False
	`!b` evaluates to False
	 The argument holds
Assume `b` is False
	`b == False` evaluates to True
	`!b` evaluates to True
	The argument holds
The argument holds for all booleans b. ∎


#### Negation:
```
P(b) = ((b == False) == ¬b)

Negation of first statement:
∃ b ∈ B, ¬P(b)

Let E(b)  =  ¬P(b)  =  ¬((b == False) == ¬b)  
					=  (b == False) ≠ ¬b
					=  (b == False) = b
```

In English:

There exists a Boolean `b` such that `b == False` evaluates to `b`

## Question 6: 

For all integers `n`, there exist integers `m1` and `m2` such that  `n` is the average of `m1` and `m2`
### Formal (a)

∀ n ∈ Z, ∃ m1, m2 ∈ Z s.t ((m1 + m2) / 2) = n

### Negation (b)

¬(∀ n ∈ Z, ∃ m1, m2 ∈ Z s.t ((m1 + m2) / 2) = n)
↳      ∃ n ∈ Z, ¬(∃ m1, m2 ∈ Z s.t ((m1 + m2) / 2) = n)
↳      ∃ n ∈ Z s.t. ∀ m1, m2 ∈ Z, ¬((m1 + m2) / 2) = n)
↳      ∃ n ∈ Z s.t. ∀ m1, m2 ∈ Z, (m1 + m2) / 2) ≠ n

There exists an integer `n` such that for all integers `m1` and `m2`, `n` is not their average

### Proof (c)

Prove:
```
∀ n ∈ Z, ∃ m1, m2 ∈ Z s.t ((m1 + m2) / 2) = n
```

Let `n` be an arbitrary integer.
	Proof by example.
	Assume `m1` = `n`
	Assume `m2` = `n`
	`m1 + m2` = `2n`
	 `2n / 2` equals `n`
We have shown that the argument is valid for any integer `n`. ∎