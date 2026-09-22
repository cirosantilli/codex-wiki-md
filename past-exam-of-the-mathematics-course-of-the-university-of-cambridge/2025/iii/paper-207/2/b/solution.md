<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The hypotheses imply $a=1/5=0.2$ and $b=1/1.25=0.8$, so $a+b=1$. Conditional on the negative result at month 1, the likelihood is the probability of remaining in $S$ at month 2 and moving to $I$ by month 3. The supplied [matrix exponential](../../../../../../matrix-exponential.md) gives

$$
P_{SS}(1)=0.8+0.2e^{-1},
\qquad
P_{SI}(1)=0.2(1-e^{-1}).
$$

The [Markov property](../../../../../../markov-property.md) therefore gives

$$
\boxed{P_{SS}(1)P_{SI}(1)
=(0.8+0.2e^{-1})0.2(1-e^{-1})
=0.16-0.12e^{-1}-0.04e^{-2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
