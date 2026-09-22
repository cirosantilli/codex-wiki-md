<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sum of the first $n/2$ variables has distribution $\operatorname{Bin}(n/2,1/2)$. For any fixed half-circle interval $I$, put

$$
D_I=\sum_{i\in I}X_i-\sum_{i\notin I}X_i,
\qquad
Z_I=\sum_{i\in I}X_i+\sum_{i\notin I}(1-X_i).
$$

The $n$ terms defining $Z_I$ are independent Bernoulli variables of parameter $1/2$, so $Z_I\sim\operatorname{Bin}(n,1/2)$ and $D_I=Z_I-n/2$. Part (b), with $h=w/n$, gives

$$
P(|D_I|\geq w)\leq2e^{-2w^2/n}.
$$

There are at most $n$ cyclic intervals of length $n/2$; this also covers the non-wrapping interpretation in the question. They need not be independent, since the [union bound](../../../../../boole-s-inequality.md) always applies. Hence

$$
P(\text{some half-circle has imbalance at least }w)
\leq2n e^{-2w^2/n}.
$$

With $w=c\sqrt{n\log n}$ and natural logarithms, this becomes $2n^{1-2c^2}$, which tends to zero for every $c>1/\sqrt2$. In particular,

$$
\boxed{c=1\text{ suffices}.}
$$

The argument proves [uniform half-circle balance for independent Bernoulli variables](../../../../../uniform-half-circle-balance-for-independent-bernoulli-variables.md). It improves on separately bounding the two half sums by recognizing the difference as one centered binomial variable.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
