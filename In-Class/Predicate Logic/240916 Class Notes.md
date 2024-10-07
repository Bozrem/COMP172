## Warm Up

A REAL NUMBER is any number on the number line like -1, pi, 2.333...

Are the following statements true or false, and why?

1. For all real numbers x, x^2 ≥ 0
	1. True because squaring any number either moves it on the number line or doesn't move it at all
2. There exists a real number `x` such that `x^2` = `x`
	1. True because 0 is a real number
3. For all real numbers `x`, `x^2` ≥ `x`
	1. False by example of `x = 0.5`
4. There exists a real number `x` such that `x^2 = -1`
	1. False, because if you use algebra to solve for `x` you create an imaginary number, which is not a real number

## Symbols

∀ - "For all"
∃ - "There exists."
∈ - "Element of"
s.t. - "Such that"

## For-all statements
"Universal Statements"

∀ x ∈ D, P(x)
For all x in the domain, statement p depending on x is true

Considered true if P(x) holds for every x in D
Considered false if there are any x in D for which P(x) does not hold

## There Exists statements
∃ x ∈ D s.t. P(x)

True if there exists at least one x in domain D in which P(x) holds
False if P(x) is false for every value of x in D

## Predicate
A statement that depends on a variable is known as a "predicate"

## Practice

Rewrite the following statements more formally

1. All triangles have three sides.
	1. Let T be all triangles
	2. Let P(t) be true when a triangle t has three sides
	3. ∀ t ∈ T, P(t)
2. No dogs have wings.
	1. Let D be all dogs
	2. Let P(d) be true when a dog d has wings
	3. ∀ d ∈ D, ¬P(d)
3. Some cars are red.
	1. Let C be all cars
	2. Let P(c) be true when a car c is red
	3. ∃ c ∈ C, P(c)
4. If a program has no loops, then it terminates
	1. Let D be all programs
	2. Let d be a program
	3. Let L(d) be if the program has loops
	4. Let T(d) be if the program terminates
	5. Let P(d) be true for the conditional L(d) → T(d)
	6. ∀ programs p, p has no loops → p terminates

## Proofs

#### How do we prove a ∀-statement?

**Theorem:** For all booleans b, the expression b == True evaluates to b

Proof:
Proof by exhaustion.
If b is False, b == True becomes False == True, which evaluates to False ✓
If b is True, b == True becomes True == True, which evaluates to True ✓
b == True evaluates to b in all cases of b. ∎


A different way to prove this is a **Proof by Arbitrary/generic element**
**Theorem:** For all integers `n`, (`n` + 1)^2 = `n`^2 + 2`n` + 1

Proof:
Let `n` be an arbitrary integer.
$(n + 1)^2 = (n + 1)(n + 1)$
    $= n(n + 1)$ + 1()
    $= 
 
