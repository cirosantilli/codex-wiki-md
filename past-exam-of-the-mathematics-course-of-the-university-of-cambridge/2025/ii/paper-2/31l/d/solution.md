<h1 id="31l/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the empirical Rademacher convention

$$
\widehat{\mathcal R}(A)
=\frac1n\mathbb E_\sigma
\sup_{a\in A}\sum_{i=1}^n\sigma_i a_i.
$$

Because $H_3$ is symmetric under $h\mapsto-h$, optimizing a linear functional over the positive $\ell^1$ hull defining $\mathcal F$ gives

$$
\widehat{\mathcal R}(\mathcal F(x_{1:n}))
\leq\widehat{\mathcal R}(H_3(x_{1:n})).
$$

By part (c), $VC(H_3)\leq D=d(d+1)/2$. Sauer--Shelah therefore bounds the number $N$ of distinct label vectors on the sample by

$$
N\leq s(H_3,n)\leq(n+1)^D.
$$

Massart's finite-class lemma states that for $A\subseteq\{-1,1\}^n$,

$$
\widehat{\mathcal R}(A)
\leq\sqrt{\frac{2\log|A|}{n}}.
$$

Applying it to the distinct label vectors of $H_3$ gives

$$
\widehat{\mathcal R}(\mathcal F(x_{1:n}))
\leq\sqrt{\frac{2D\log(n+1)}n}
=\boxed{\sqrt{\frac{(d^2+d)\log(n+1)}n}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31L](../../31l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
