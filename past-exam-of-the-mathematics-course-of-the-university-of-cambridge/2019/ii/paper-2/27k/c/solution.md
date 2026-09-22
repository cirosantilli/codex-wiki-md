<h1 id="27k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After leaving zero, the jump chain avoids every future reset with probability

$$
q=\prod_{i=1}^{\infty}\frac1{1+\rho_i}.
$$

This probability is positive exactly when $\prod_{i\geq1}(1+\rho_i)<\infty$. If $q>0$, the probability of ever returning to zero is less than one, so the irreducible chain is transient. If $q=0$, a reset to zero occurs almost surely after each departure; by the [Strong Markov property](../../../../../../strong-markov-property.md) this happens repeatedly, so the chain is recurrent. Therefore

$$
\boxed{X\text{ is transient}\iff\prod_{i=1}^{\infty}(1+\rho_i)<\infty.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
