# Definitions
**Proposition** - Any declarative statement that is either true or false
**Well Formed Formula (WFF)** - Formula using correct syntax of logic
**Truth Table** - Method of solving complex WFFs that simulates each situation of its basic elements
**T - Tautology** - a statement which is always true. Like if you map this out on a truth table then its like a “Taut” line
**丄 - Contradictory** - a statement which is always false. It contradicts itself and cannot be true
**P - Contingent** - a statement with at least one of each. Its a contingency, like “it depends”
**Predicate** - A function taking 1 or more inputs outputting true or false


# Notes
### Propositions
* Can be true or false, usually in CS we use 0 for False, 1 for True
* We can combine them with operators like:
	* ¬  not
	* ∧  and
	* ∨  or
	* → as an If-Then statement
	* ↔ as an If and only If then statement
## Well Formed Formulas (WFF)
* Propositions cannot be with each other without an operator
* Operators must have both Propositions (except ¬)
* An operator cannot touch an operator
* Parenthesis () are used to mark each part of a WFF
* EXAMPLES:
	* (P ∧ ¬Q)
	* ¬P
	* ((P → Q) ∧ (P ∨ Q)) ∨ ¬Q
	* Q
* Any WFF is either a single thing or made of multiple other WFFs
* This property allows us to make tree diagrams of our WFFs
## Truth Tables 
* Lists every possibility of its simple propositions
* Example below

| P   | Q   | P ∧ Q | ¬Q  | (P ∧ Q) ∨ ¬Q |
| --- | --- | ----- | --- | ------------ |
| 0   | 1   | 0     | 0   | 0            |
| 0   | 0   | 0     | 1   | 1            |
| 1   | 1   | 1     | 0   | 1            |
| 1   | 0   | 0     | 1   | 1            |
## Understanding If-Then as a conditional
Initially, I had some trouble when faced with a truth table like below. The way that I have to make myself think about it is as a promise.
Lets make this case with the following simple propositions
* P is "God Exists"
* Q is "I pray"
Both of these are propositions, and God can either exist or not, and I can either pray or not pray.
In this, my promise (P → Q) becomes
* If God exists, I will pray
So lets do each scenario
* Q, P
* 0, 0 - God does not exist, I do not pray. I was never obligated to anything if God does not exist. I've kept my promise. WFF is 1
* 0, 1 - God does not exist, I pray anyway. Still was not obligated to doing anything. Praying does not break my promise. WFF is 1
* 1, 1 - God exists, and I pray. I've kept my promise. WFF is 1
* 1, 0 - God exists, but I don't pray out of spite. I've broken my promise. WFF is 0

| Q   | P   | P → Q |
| :-- | --- | ----- |
| 0   | 1   | 1     |
| 0   | 0   | 1     |
| 1   | 1   | 1     |
| 1   | 0   | 0     |

## Logical Equivalence
I found some practice tables for these, and it came up with a very interesting (ρ→!ρ). I want to think out this scenario as well. Lets do ρ is “I get a 4.0”
* P is true. I got a four point, so then my promise is that I didn’t get a four point, but I did, so this is false.
* P is false. I didn’t get a four point, so my promise is kept either way what the second one did. This is true

In this, the truth table ends up just being the same numbers as just ¬P

That makes P → ¬P logically equivalent to ¬P

## Predicate Logic
An extension of Prepositional Logic to use functions
It takes