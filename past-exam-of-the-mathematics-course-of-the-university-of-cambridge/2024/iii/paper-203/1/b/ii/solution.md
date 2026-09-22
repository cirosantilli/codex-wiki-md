<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $r\geq1$, let $R_r=[-r,r]\times(0,1]$. The [Brownian representation of half-plane capacity](../../../../../../../brownian-representation-of-half-plane-capacity.md) gives

$$
\operatorname{hcap}(R_r)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

On hitting $R_r$ the imaginary part is at most one, while the [harmonic measure](../../../../../../../harmonic-measure.md) estimate supplied in the question shows that the probability of reaching a disc of radius $O(r)$ containing $R_r$ is $O(r/y)$. Hence $\operatorname{hcap}(R_r)\leq Cr$, the [half-plane capacity of a low rectangle](../../../../../../../half-plane-capacity-of-a-low-rectangle.md) bound.

Set

$$
A_n=n^{-1}R_n=[-1,1]\times(0,n^{-1}].
$$

The [scaling and translation of half-plane capacity](../../../../../../../scaling-and-translation-of-half-plane-capacity.md) gives

$$
\operatorname{hcap}(A_n)=n^{-2}\operatorname{hcap}(R_n)\leq Cn^{-1}\longrightarrow0,
$$

whereas $\operatorname{diam}(A_n)=\sqrt{4+n^{-2}}\to2$. This supplies the required sequence.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
