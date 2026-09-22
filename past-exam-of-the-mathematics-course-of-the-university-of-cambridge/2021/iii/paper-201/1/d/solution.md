<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $S=X_1+X_2$. By symmetry,

$$
\mathbb E[X_1\mid S]=\mathbb E[X_2\mid S].
$$

Their sum is $S$, which is measurable with respect to $\mathcal G=\sigma(S)$, so

$$
2\mathbb E[X_1\mid\mathcal G]
=\mathbb E[X_1+X_2\mid\mathcal G]
=S.
$$

Therefore

$$
\boxed{\mathbb E[X_1\mid\mathcal G]=\frac{X_1+X_2}{2}}.
$$

This also follows from the [Gaussian conditional expectation](../../../../../../gaussian-conditional-expectation.md) formula because $\operatorname{Cov}(X_1,S)/\operatorname{Var}(S)=1/2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
