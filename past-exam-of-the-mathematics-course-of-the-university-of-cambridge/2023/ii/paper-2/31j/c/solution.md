<h1 id="31j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The functions $x\mapsto x^T\beta$ form a real vector space of dimension $p$. Hence the [VC dimension of a vector space](../../../../../../vc-dimension-of-a-vector-space.md) gives

$$
\operatorname{VC}(\mathcal H_{\mathcal F_1})\leq p.
$$

Applying the [Sauer-Shelah lemma](../../../../../../sauer-shelah-lemma.md) and then the [Sauer-Shelah growth bound](../../../../../../sauer-shelah-growth-bound.md),

$$
s(\mathcal H_{\mathcal F_1},n)
\leq\sum_{j=0}^p\binom nj
\leq\boxed{(n+1)^p}.
$$

This is the [growth bound for homogeneous linear classifiers](../../../../../../growth-bound-for-homogeneous-linear-classifiers.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
