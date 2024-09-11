## Warm up
p = "I am exercising"
q = "My heart rate is over 100"

Argument:
```
p → q
¬q
∴ ¬p
```

| p   | q   |     | p → q | ¬q  |     | ¬p  |
| --- | --- | --- | ----- | --- | --- | --- |
| ==0==   | ==0==   |     | ==1==     | ==1==   |     | ==1==   |
| 0   | 1   |     | 1     | 0   |     | 1   |
| 1   | 0   |     | 0     | 1   |     | 0   |
| 1   | 1   |     | 1     | 0   |     | 0   |
Since the arguments only critical row of p=0, q=0 has a true conclusion, the argument is valid

## Proving Arguments
A truth table can get really big if there are a lot of variables, so it may not be the best way to look at it.

Instead, we can PROVE that an argument is true.


* A Proof is a series of arguments, which we call **steps**
* Each Step is an argument, but they should be simple
* Each Step must be valid
* The hypotheses of each step must be either 
	* Hypotheses of the whole argument
	* Previously proven in steps
### Example Proof
```
q → r
p
¬q → ¬p
∴ r ∧ p
```
You can convert things to other logically equivalent versions of itself. 

In the example above, the contrapositive of `¬q → ¬p` is `p → q`

Proof:
Since `¬q → ¬p`, we also have `p → q` (contrapositive)
Since `p` holds and `p → q`, `q` holds also
Then since `q` holds and `q → r`, `r` holds as well
Since `r` holds and `p` holds, `r ∧ p` holds. ■

You can end a proof with some sort of symbol.

## Rules of Inference
Standard arguments that you may use in proofs.
#### Modus Ponens
```
p → q
p
∴ q
```

#### Modus Tollens
```
p → q
¬q
∴ ¬p
```
\
#### ∧-Introducion
```
p
q
∴ p ∧ q
```

#### ∧-Elimination
```
p ∧ q
∴ p
```

#### ∨-Introduction
```
p
∴ p ∨ q
```

#### ∨-Elimination
```
p ∨ q
p → r
q → r
∴ r
```

## Practice
#### Challenge 
Argument to prove:
```
¬p ∧ s
q ∨ ¬r
s → r
∴ q ∨ p
```

Proof:
Since `¬p ∧ s`, `s` holds.
Since `s` holds, and `s → r`, `r` must also hold
Since `¬r` is false, `q ∨ ¬r` means q must hold
Since `q` holds, `q ∨ p` also holds. ∎

#### In class
```
p → q
p → ¬r
p
∴ q ∧ ¬r
```

Proof:
Since `p`,  `p → q` makes `q` hold
Since `p`, `p → ¬r` makes `¬r` hold
Since `¬r` holds and `q` holds, `q ∧ ¬r` holds. ∎


