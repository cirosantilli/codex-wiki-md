<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
A(x)=\sum_{p\leq x}\frac{\log p}{p}=\log x+E(x),
\qquad E(x)=O(1).
$$

The [Abel summation formula](../../../../../../abel-s-summation-formula.md) with weight $1/\log t$ gives

$$
\sum_{p\leq x}\frac1p
=\frac{A(x)}{\log x}
+\int_2^x\frac{A(t)}{t(\log t)^2}\,dt.
$$

Substituting $A(t)=\log t+E(t)$ yields

$$
\sum_{p\leq x}\frac1p
=\log\log x+c+\frac{E(x)}{\log x}
-\int_x^\infty\frac{E(t)}{t(\log t)^2}\,dt
$$

for a constant $c$. Both final terms are $O(1/\log x)$, so

$$
\boxed{\sum_{p\leq x}\frac1p
=\log\log x+c+O\left(\frac1{\log x}\right).}
$$

This is the [Mertens second theorem](../../../../../../mertens-second-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
