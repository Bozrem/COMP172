## Quotient-Remainder Theorem

### Definition

For any integer n and positive integer d, there exist unique integers q and r such that n = dq + r and 0 ≤ r < d

∀ n ∈ ℤ, ∀ d ∈ ℕ, (∃ q, r ∈ ℤ s.t. (`n = dq + r` ∧ `0 ≤ r < d`))

### Examples

Prove:    ∀ n ∈ ℤ, $n^2 - n$ is even

By the quotient remainder theorem (d=2), ∃ q, r ∈ ℤ s.t. $n = 2q + r$ , $0 ≤ r < 2$
So $n = 2q$ or $n = 2q +1$ 
Let $n = 2q$
	$n^2 - n = (2q)^2 - (2q)$
	$= 4q^2 - 2q$
	$= 2(2q^2 - q)$, which is even
Let $n = 2q + 1$
	$n^2 - n = (2q + 1)^2 - (2q + 1)$
	$=4q^2 + 4q + 1 - 2q - 1$
	$= 4q^2 + 2q$
	$= 2(2q^2 + q)$, which is even
So in all cases, $n^2 - n$ is even. ∎

