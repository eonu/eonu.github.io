[TOC]

# Combinatorics and counting

## Product rule

If $A$ and $B$ are finite sets, then $|A \times B|=|A|\cdot|B|$.

**Proof:** Obvious, but prove with induction on $|A|$.

### General product rule

If $A_1, A_2, \ldots, A_m$ are finite sets, then
$$
|A_1 \times A_2 \times \ldots \times A_m|=|A_1|\cdot|A_2|\cdot \ldots \cdot |A_m|
$$
**Proof:** Induction on $m$, using the basic product rule.

## Counting subsets

A finite set, $S$, has $2^{|S|}$ distinct subsets.

**Proof:** Suppose $S = \{s_1, s_2,\ldots, s_m\}$.
There is a one-to-one correspondence (bijection), between subsets of $S$ and bit strings of length $m = |S|$.
The bit string of length $|S|$ we associate with a subset $A ⊆ S$ has a $1$ in
position $i$ if $s_i ∈ A$, and $0$ in position $i$ if $s_i \not \in A$, for all $i ∈ \{1,\ldots, m\}$.

By the product rule, there are $2^|S|$ such bit strings.

## Counting functions

### Number of functions

For all finite sets $A$ and $B$, the number of distinct functions, $F : A \to B$, mapping $A$ to $B$ is:
$$
|B|^{|A|}
$$
**Proof:** Suppose $A = \{a_1,\ldots, a_m\}$.
There is a one-to-one correspondence between functions $f : A → B$ and strings (sequences) of length $m = |A|$ over an alphabet of size $n = |B|$.

By the product rule, there are $n^m$ such strings of length $m$.

## Inclusion-exclusion principle

For any finite sets $A$ and $B$ (not necesarily disjoint):
$$
|A\cup B|=|A|+|B|-|A\cap B|
$$

## Generalized pigeonhole principle

### Theorem

If $N \geq 0$ objects are placed in $k \geq 1$ boxes, then at least one box contains at least $\lceil \frac{N}{k} \rceil$ objects.

### Proof

Suppose no box has more than $\lceil \frac{N}{k} \rceil-1$ objects. Sum up the number of objects in the $k$ boxes. It is at most
$$
k \cdot \left(\left\lceil\frac{N}{K} \right\rceil-1\right) < k \cdot \left(\left(\frac{N}{k}+1\right)-1\right)=N
$$
Thus, there must be fewer than $N$. Contradiction.

> E.g. "At least $d$ students in this course were born in the same month"
>
> Suppose the number of students registered for the course is $145$.
>
> What is the maximum number $d$ for which **it is certain** that the statement is true?

#### Solution

Since we are assuming there are $145$ registered students, $\lceil \frac{145}{12}\rceil=13$, so by GPP we know that the statement is true for $d=13$.

## Permutations

A **permutation** of a set $S$ is an ordered arrangement of the elements of $S$. i.e. A sequence containing every element of $S$ exactly once.

## $k$-permutations

A $k$-permutation of a set $S$ is an ordered arrangement of $k$ distinct elements of $S$.

If we have a set of size $n$, the number of $k$-permutations of the $n$-set are the different ordered arrangements of a $k$-element subset of the set with $n$ elements. This is given by:
$$
\frac{n!}{(n-k)!}
$$

> E.g. how many ways can first and second place be awarded to 10 people?
>
> Here, we have $n=10$ and $k=2$. 
>
> Order does matter in this case, because someone coming first and another person coming second is not the same, the other way round.
>
> Therefore, we have to find the $2$-permutations of $10$ elements.
>
> $\frac{10!}{(10-2)!}$

## Combinations

A $k$-element combination of the set with $n$ elements is a $k$-element subset, in which the elements are not ordered. The number of $k$-element combinations of the set with $n$ elements is given by:
$$
\binom{n}{k}=\frac{n!}{(n-k)!k!}
$$

> E.g. How many different 5-card poker hands can be dealt from a deck of $52$ cards?
>
> $\binom{52}{5}$

> E.g. How many different 47-card poker hands can be dealt from a deck of $52$ cards?
>
> $\binom{52}{47}$

## Binomial theorem

$$
\forall n\geq 0, \quad (x+y)^n=\sum_{r=0}^n \binom{n}{r}x^{n-r}y^r
$$

## $k$-combinations with repetition

To choose $k$ elements **with repetition allowed** from a set of size $n$, we can do this in the following number of ways:
$$
\binom{n+r-1}{r}=\binom{n+r-1}{n-1}
$$

> E.g. How many different solutions in non-negative integers $x_1$,$x_2$ and $x_3$ does the following equation have?
>
> $$x_1+x_2+x_3=11$$

**Solution:** We have to place $11$ pebbles into three different bins $x_1$, $x_2$ and $x_3$.

This is the equivalent to choosing an $11$-combination (with repetition) from a set of size $3$, so the answer is:
$$
\binom{11+3-1}{11}
$$

## Summary

| Type             | Repetition allowed? | Formula                                  |
| ---------------- | ------------------- | ---------------------------------------- |
| $r$-permutations | No                  | $\displaystyle\frac{n!}{(n-r)!}$         |
| $r$-combinations | No                  | $\displaystyle\frac{n!}{(n-r)!r!}=\binom{n}{r}$ |
| $r$-permutations | Yes                 | $n^r$                                    |
| $r$-combinations | Yes                 | $\displaystyle\frac{(n+r-1)!}{r!(n-1)!}=\binom{n+r-1}{r}$ |

## Useful example questions

**Question:** How many solutions are there to the equation $x_1+x_2+x_3+x_4+x_5+x_6=29$ where $x_i$ ($i=1,2,3,4,5,6$) is a non-negative integer, such that $x_i>1$ for $i=1,2,3,4,5,6$.

**Answer:** Let $x_i=y_i+2 \iff y_i=x_i-2$ for $i=1,2,3,4,5,6$. Then, we obtain
$$
y_1+y_2+y_3+y_4+y_5+y_6=29-6\cdot 2=17
$$
Where $y_i$ is now a non-negative number for $i=1,2,3,4,5,6$. The number of solutions to this equation can now be reduced to solving a typical stars and bars problem:
$$
\binom{17+6-1}{6-1}=\binom{22}{5}
$$

---

**Question:** How many solutions are there to the equation $x_1+x_2+x_3+x_4+x_5+x_6=29$ where $x_i$ ($i=1,2,3,4,5,6$) is a non-negative integer, such that $x_1 \leq 5$.

**Answer:** If $x_1$ is fixed, then the number of solutions for the other variables is:
$$
\binom{5+(29-x_1)-1}{5-1} \quad \text{or} \quad \binom{5+(29-x_1)-1}{(29-x_1)}
$$
Since the solutions are in one-to-one correspondence with the reorderings of $29-x_1$ stars and $5-1=4$ bars.

The possible values for $x_1$ are $0,1,2,3,4,5$ and hence, the answer is:
$$
\sum_{k=0}^5\binom{5+(29-k)-1}{4}
$$

---

Give a formula for the coefficient of $x^k$ in the expansion of $(x+\frac{1}{x})^{100}$, where $k$ is an integer.

**Answer:** We know that:
$$
\text{Coefficient of} \ x^{n-r}y^r=\binom{n}{r}, \ \text{where} \ y=\frac{1}{x}
$$

$$
x^{n-r}\cdot \frac{1}{x^r}=x^k \\
n-2r=k \\
r=\frac{n-k}{2}
$$

Coefficient of $x^k$ in the expansion of $(x+\frac{1}{x})^n$ is $\binom{n}{\frac{n-k}{2}}$.

Formula for the coefficient of $x^k$ in the expansion of $(x+\frac{1}{x})^{100}$ is $\binom{100}{\frac{100-k}{2}}$.

---

Give a formula for the coefficient of $x^k$ in the expansion of $(x-\frac{1}{x})^{100}$ where $k$ is an integer.

**Answer:** A general term in this expression is of form:
$$
\binom{100}{r}x^{100-r}(-\frac{1}{x})^r=\binom{100}{r}x^{100-2r}(-1)^r
$$
For all integers $k$ such that $k=100-2r$. Rearranging for $r$ gives: $r=\frac{100-k}{2}$.

The coefficient is $ \displaystyle\binom{100}{\frac{100-k}{2}}(-1)^\frac{100-k}{2}$  .
