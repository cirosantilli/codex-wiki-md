<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [homogenization of Dirichlet boundary data](../../../../../../homogenization-of-dirichlet-boundary-data.md): put $v=u-\varphi$, using the supplied extension of $\varphi$ to the half-ball. Then $v=0$ on the flat face and $\Delta v=f-\Delta\varphi$. The [second-derivative estimate at a flat Dirichlet boundary](../../../../../../second-derivative-estimate-at-a-flat-dirichlet-boundary.md) from part (a) gives

$$
\|v\|_{W^{2,2}(B_1^+)}
\leq C(n)\left(\|v\|_{W^{1,2}(B_2^+)}+\|f-\Delta\varphi\|_{L^2(B_2^+)}\right).
$$

The [triangle inequality](../../../../../../triangle-inequality.md) gives $\|v\|_{W^{1,2}}\leq\|u\|_{W^{1,2}}+\|\varphi\|_{W^{1,2}}$, while the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds $\|\Delta\varphi\|_{L^2}$ by $\sqrt n\|D^2\varphi\|_{L^2}$. Finally $u=v+\varphi$, so restriction from the larger half-ball and another [triangle inequality](../../../../../../triangle-inequality.md) give

$$
\boxed{\|u\|_{W^{2,2}(B_1^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_2^+)}+\|f\|_{L^2(B_2^+)}+\|\varphi\|_{W^{2,2}(B_2^+)}\right).}
$$

**Nonzero boundary data contribute the second-order Sobolev norm of their extension.** No estimate for a separately constructed extension is needed, because $\varphi$ is already given on the half-ball.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
