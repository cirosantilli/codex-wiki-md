<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $k\geq0$, take $f_k(x)=\mathbf1_{\{x\geq k+1\}}$ and write $q_k=\mathbb P(X\geq k+1)$. Since $f_k^2=f_k$,

$$
\operatorname{Ent}(f_k(X)^2)=-q_k\log q_k.
$$

Its discrete derivative is nonzero only at $k$, so

$$
\mathbb E|Df_k(X)|^2=\mathbb P(X=k)=p_k.
$$

For a [Poisson distribution](../../../../../../poisson-distribution.md), $p_{k+1}/p_k=\lambda/(k+1)$ and $q_k\sim p_{k+1}$ as $k\to\infty$. Hence

$$
\frac{-q_k\log q_k}{p_k}
\sim\frac{\lambda}{k+1}\log\frac1{p_{k+1}}
\sim\lambda\log k\longrightarrow\infty,
$$

where the final estimate follows from [Stirling formula](../../../../../../stirling-formula.md). No finite constant $C$ can therefore make the proposed inequality hold for every $f$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
