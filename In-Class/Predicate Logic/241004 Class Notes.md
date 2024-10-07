## Warm Up

Prove: Let $d$ be an integer such that $d > 1$. If $d$ divides $n$, then $d$ does not divide $(n + 1)$

Let $d$ be an integer > 1.
Assume $d|n$
Since $d | n$, $n = ad$ for some $a$ ∈ ℤ
So $n + 1 = ad + 1$
By quotient remainder theorem, $ad + 1$ is not divisible by $d$ for a $d > 1$

## Euclid's Stuff

Theorem: If r ∈ ℚ, then ∃ a, b ∈ ℤ s.t. $r = a/b$ and $b > 0$

Ex: $2 = -6 /-3 = 6/3$ 

Proof:
Assume $r$ is rational
Then $r = c / d$ for some c, d ∈ ℤ and $d ≠ 0$
We have two cases
Case 1: $d > 0$
	Set $a = c$ and $b = d$ so that $r = a / b$ and $b > 0$	
Case 2: $d < 0$
	Set $a = -c$ and $b = -d$ so that $r = -a / -b = a / b$ and $b > 0$



Theorem: $\sqrt2$ is irrational

Assume for contradiction $\sqrt2$ is rational.
	So $\sqrt2 = a / b$ for some a, b ∈ ℤ and $b > 0$. (By previous theorem)
	$\sqrt2 * b = a$
	$2b^2 = a^2$
	$a$ is even, since $a^2$ is even (By proof last class)
	So $a = 2 * a_1$ for some $a_1$ ∈ ℤ
	So $2b^2 = (2 * a_1)^2$ 
	So $b^2 = 2a_1^2$
	$b$ is also even, since $b^2$ is even (By proof last class)
	So $b = 2b_1$ for some $b_1$ ∈ ℤ
	So $(2b_1)^2 = 2a_1^2$
	So $2b_1^2 = a_1^2$
	If we continue, we get an infinite decreasing sequence of positive **integers**, with each step down being half its previous.
	This is a contradiction, so $\sqrt2$ is irrational. ∎