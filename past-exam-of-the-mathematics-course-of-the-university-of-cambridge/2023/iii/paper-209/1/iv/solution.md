<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let the square contain the Euclidean ball of radius $R$, set $r_x=\max(1,\lVert x\rVert)$, and define the logarithmic cutoff

$$
\varphi_x=
\begin{cases}
1,&r_x=1,\\
\dfrac{\log(R/r_x)}{\log R},&1<r_x<R,\\
0,&r_x\geq R.
\end{cases}
$$

Then $\varphi_0=1$ and $\varphi=0$ on the boundary. On an edge at radius comparable to $r$, the [mean value theorem](../../../../../../mean-value-theorem.md) gives $|\varphi_x-\varphi_y|\leq C/(r\log R)$. There are $O(r)$ edges in the annulus of radius $r$, hence the [discrete Dirichlet energy](../../../../../../discrete-dirichlet-energy.md) satisfies

$$
\sum_{xy\in\bar E}(\varphi_x-\varphi_y)^2
\leq\frac C{(\log R)^2}\sum_{r=1}^{R}\frac1r
\leq\frac C{\log R}\longrightarrow0.
$$

This logarithmic cutoff is the discrete manifestation of recurrence in two dimensions.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
