<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $\overline X_n\sim N(\mu,1/n)$,

$$
\mathbb E T_n=\mathbb E\overline X_n^2
=\mu^2+\frac1n,
$$

so

$$
\boxed{\operatorname{Bias}(T_n)=\frac1n}.
$$

Every leave-one-out mean has variance $1/(n-1)$, and hence

$$
\mathbb E\widehat B_n
=(n-1)\left(\frac1{n-1}-\frac1n\right)
=\frac1n.
$$

Therefore

$$
\boxed{\operatorname{Bias}(\widetilde T_{\rm JACK})=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
