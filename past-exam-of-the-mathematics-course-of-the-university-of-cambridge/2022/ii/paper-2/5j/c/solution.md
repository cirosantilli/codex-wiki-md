<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [log-likelihood](../../../../../../log-likelihood.md) has derivative

$$
\ell'(\theta)=\sum_iY_i-nA'(\theta).
$$

Differentiating the normalizing identity for the family gives

$$
A'(\theta)=\mathbb E_\theta Y_1=\mu(\theta),
\qquad
A''(\theta)=\operatorname{Var}_\theta(Y_1)\geq0.
$$

Hence an interior maximum satisfies, and under nondegeneracy uniquely satisfies,

$$
\boxed{\mu(\widehat\theta_{\rm MLE})=\overline Y}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
