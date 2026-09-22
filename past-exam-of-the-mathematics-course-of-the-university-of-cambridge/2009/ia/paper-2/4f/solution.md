<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The events $B\cap A_i$ are pairwise disjoint and their union is $B$. Finite additivity and the definition of [conditional probability](../../../../../conditional-probability.md) therefore give the [law of total probability](../../../../../law-of-total-probability.md):

$$
P(B)=\sum_{i=1}^nP(B\cap A_i)
=\sum_{i=1}^nP(A_i)P(B\mid A_i).
$$

For the [birthday problem](../../../../../birthday-problem.md), let $D$ mean that all birthdays differ. For $n\leq365$, sequential conditioning on previous distinct birthdays and [independence of random variables](../../../../../independent-random-variables.md) give

$$
P(D)=\prod_{j=0}^{n-1}\left(1-\frac{j}{365}\right)
\leq\exp\left(-\sum_{j=0}^{n-1}\frac{j}{365}\right)
=\exp\left(-\frac{n(n-1)}{730}\right).
$$

Here each factor uses the stated bound $1-x\leq e^{-x}$. For $n\geq29$, $n(n-1)\geq812>730\log3$, so

$$
\boxed{P(\text{at least one shared birthday})=1-P(D)\geq\frac23.}
$$

For $n>365$ a match is certain by the [pigeonhole principle](../../../../../pigeonhole-principle.md). The threshold from the exponential bound is $(1+\sqrt{1+2920\log3})/2\approx28.8$, so $29$ suffices.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
