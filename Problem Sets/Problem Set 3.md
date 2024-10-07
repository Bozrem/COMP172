## Question 1: Difference of Odds

Prove that the difference between any two odd numbers is even.

Proof:
Let $a$, $b$ be arbitrary odd integers
$a = 2n + 1$ for $n$ ∈ ℤ
$b = 2m + 1$ for $m$ ∈ ℤ
Then $a - b = (2n + 1) - (2m + 1)$
$= 2n - 2m$
$= 2(n - m)$
So $a - b$ is even. ∎

## Question 2: Rational Squares

Prove that for all real numbers $r$, if $r$ is rational, so is $2r^2$.

Proof:
Let $r$ be an arbitrary rational number
So $r = \frac{a}{b}$ for some $a$, $b$ ∈ ℤ, $b \neq 0$
Then $2r^2 = 2\frac{a}{b}^2$
$= \frac{2a^2}{b}$
$2a^2$ is an integer, and $b$ is still an integer $\neq 0$ 
$2r^2$ is rational. ∎

## Question 3: T or F Proofs

#### For all integers $m$, $n$, if $m$ is even, and $4 | mn$, then $n$ is even

**TRUE**

Proof:
Let $m$, $n$ be arbitrary integers
Assume $m$ is even, such that $m = 2a$ for some $a$ ∈ ℤ
Assume for contradiction $n$ is odd, such that $n = 2b + 1$ for some $b$ ∈ ℤ
Then $mn = (2a)(2b + 1)$
$= 4ab + 2a$
Since $a$ is an arbitrary integer, $2a$ is not always divisible by four, making a contradiction. ∎

#### For all integers $m$, $n$, if $m$ is even, and $4 \nmid mn$, then $n$ is not even

Proof:
Let $m$, $n$ be arbitrary integers
Assume $m$ is even, such that $m = 2a$ for some $a$ ∈ ℤ
Assume $4 \nmid mn$
Then $4 \nmid 2an$
Then $2 \nmid an$
Assume for contradiction that $n$ is even, such that $n = 2b$, $n$ ∈ ℤ
Then $2 \nmid 2ab$, which is a contradiction. ∎

## Question 4: ∀ $n$ ∈ ℤ, $3 \nmid n^2 - 2$

Prove that there is no integer $n$ such that $n^2 - 2$ is divisible by $3$

Proof:
We have three cases of $n$:
Case 1: $n\mod 3  = 0$
	$n$ can be written as $n = 3a$ for some $a$ ∈ ℤ
	So $n^2 = 9a^2$
	So $3 \nmid 9a^2 - 2$, which holds.
Case 2: $n \mod 3 = 1$
	$n$ can be written as $n = 3b + 1$ for some $b$ ∈ ℤ
	So $n^2 = 9b^2 + 6b + 1$
	So $3 \nmid 9b^2 + 6b - 1$, which holds.
Case 3: $n \mod 3 = 2$
	$n$ can be written as $n = 3c + 2$ for some $c$ ∈ ℤ
	So $n^2 = 9c^2 + 12c + 4$
	So $3 \nmid 9c^2 + 12c + 2$, which holds.
All possible cases of $n$ hold. ∎


## Question 5: Python Proof

```
def f(x):
	if x > 0:
		return x + 10
	else:
		return 2 * x
```

#### ∀ $x$ ∈ ℤ, ($x > 0$ ∧ $f(x) > 0$) ∨ ($x ≤ 0$ ∧ $f(x) ≤ 0$)

Proof:
Let $x$ be an arbitrary integer
There are three cases:
Case 1: $x > 0$
	$f(x)$ returns $x + 10$
	$x + 10 > x > 0$, so this case holds
Case 2: $x = 0$
	$f(x)$ returns $2x$
	$2x = 0 ≤ 0$, so this case holds
Case 3: $x < 0$
	$f(x)$ returns $2x$
	Positive $*$ negative → negative, so this case holds.
All possible cases of $x$ hold. ∎

#### ∀ $x$ ∈ ℤ, $f(x) \neq 5$

Proof:
Let $x$ be an arbitrary integer
There are three cases:
Case 1: $x > 0$
	The smallest integer $x$ can be in this case is 1
	For the smallest input, $x + 10 = 11$ is the output, which is always larger than 5.
Case 2: $x = 0$
	$f(x)$ returns $2x$, which is $0 \neq 5$
Case 3: $x < 0$
	$f(x) returns $2x$
	Positive $*$ negative → negative, which cannot be $5$.
All possible outputs of $f(x)$ cannot be $5$. ∎

## Question 6

$a + b + c = 0$, where $a$, $b$, $c$ are all real numbers
#### Is it possible that all three of $a$, $b$, $c$ are rational?

Yes

Proof by example:
Let $a = \frac{2}{1}$, $b = \frac{-2}{1}$, $a = \frac{0}{1}$
$a + b + c = 0$. ∎
#### Is it possible that exactly two of $a$, $b$, $c$ are rational, and the other is irrational?

No

Proof Contradiction:
Let $c$ be an arbitrary irrational number
Let $a$, $b$ be arbitrary rational numbers such that $a - b = \frac{x}{y}$ , for some $x$, $y$ ∈ ℤ
So $\frac{x}{y} = -c$
So $\frac{-x}{y} = c$, which is a contradiction since $c$ is meant to be irrational. ∎

#### Is it possible that exactly one of $a$, $b$, $c$ are rational, and the other two are irrational?

Yes

Proof by example:
Let $a = \frac{0}{1}$, which is rational
Let $b = -\sqrt{2}$
Let $c = \sqrt{2}$
$a + b + c = 0$. ∎

#### Is it possible that all three of $a$, $b$, $c$ are irrational

Yes

Proof by example:
Let $a, b = \pi$
Let $c = -2\pi$
$a + b + c = 0$. ∎