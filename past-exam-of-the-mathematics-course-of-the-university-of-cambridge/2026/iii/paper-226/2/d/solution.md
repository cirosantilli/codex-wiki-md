<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The field $\psi$ is centered and jointly [Gaussian](../../../../../../gaussian-random-field.md). Since the [Gaussian free field](../../../../../../gaussian-free-field.md) has covariance $\mathbb E[\varphi_x\varphi_y]=g(x,y)$ and $h_x=g(x,0)/g(0,0)$,

$$
\begin{aligned}
\mathbb E[\psi_x\psi_y]
&=g(x,y)-h_xg(0,y)-h_yg(x,0)+h_xh_yg(0,0)\\
&=g(x,y)-\frac{g(x,0)g(0,y)}{g(0,0)}.
\end{aligned}
$$

Also $\psi_0=0$ and

$$
\mathbb E[\psi_x\varphi_0]=g(x,0)-h_xg(0,0)=0.
$$

Joint Gaussianity turns this zero [covariance](../../../../../../covariance.md) into independence. Therefore $\psi$ is a [Pinned Gaussian free field](../../../../../../pinned-gaussian-free-field.md) at $0$, independent of $\varphi_0$, with covariance equal to the Green function of the walk killed on hitting $0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
