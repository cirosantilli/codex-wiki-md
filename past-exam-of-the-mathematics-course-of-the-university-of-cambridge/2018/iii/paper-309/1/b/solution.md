<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the numerator in the original PDF: it contains all $n+1$ squared differentials. The local TeX ends that numerator at $n-1$, which would not give the stated [Riemannian metric](../../../../../../riemannian-metric.md).

For the [pullback of a Riemannian metric](../../../../../../pullback-of-a-riemannian-metric.md), substitute the embedding $\pi(y)=(y_1,\ldots,y_n,1)$. Its differential sends a tangent vector $v$ to $(v_1,\ldots,v_n,0)$, so $dX_i=dy_i$ for $i\le n$ and $dX_{n+1}=0$. Consequently

$$
\boxed{g=\pi^*G=\frac{\sum_{i=1}^n dy_i^2}{1+\sum_{i=1}^n y_i^2},\qquad
g_{ij}(y)=\frac{\delta_{ij}}{1+|y|^2}.}
$$

The denominator is everywhere positive. For any nonzero tangent vector,

$$
g_y(v,v)=\frac{|v|^2}{1+|y|^2}>0,
$$

so this is indeed a smooth positive-definite [Riemannian metric](../../../../../../riemannian-metric.md) on $U$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
