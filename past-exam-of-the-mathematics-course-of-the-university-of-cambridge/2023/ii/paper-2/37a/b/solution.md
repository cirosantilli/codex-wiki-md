<h1 id="37a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [mean](../../../../../../expected-value.md) extension in an ensemble of $A$ molecules is

$$
L=\frac1A\sum_i a_i l_i,
$$

with constraints $\sum_i a_i=A$ and $\sum_i a_i l_i=AL$. For occupancies $\{a_i\}$, the number of assignments of the $A$ distinguishable ensemble members to the states is the [multinomial coefficient](../../../../../../multinomial-coefficient.md)

$$
W=\frac{A!}{\prod_i a_i!}.
$$

Thus maximizing the probability at fixed $A$ and $L$ is equivalent to maximizing the stated [Lagrange multiplier](../../../../../../lagrange-multiplier.md) expression.

Because $A\gg1$, the [Stirling formula](../../../../../../stirling-formula.md) gives $\log(a_i!)\simeq a_i\log a_i-a_i$. Differentiating with respect to each $a_i$ gives

$$
-\log a_i+\tau l_i-\alpha=0,
\qquad
a_i=e^{-\alpha}e^{\tau l_i}.
$$

Normalization by $\sum_i a_i=A$ therefore yields the [probability mass function](../../../../../../probability-mass-function.md)

$$
\boxed{p_i=\frac{a_i}{A}=\frac{e^{\tau l_i}}{Z}},
\qquad
\boxed{Z=\sum_i e^{\tau l_i}}.
$$

Here $Z$ is the fixed-tension [partition function](../../../../../../canonical-partition-function.md) that normalizes the probabilities.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37A](../../37a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
