<h1 id="9a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the [spherical coordinate system](../../../../../../spherical-coordinate-system.md)

$$
\mathbf x=(r\sin\theta\cos\phi,\,
r\sin\theta\sin\phi,\,
r\cos\theta)
$$

gives the orthogonal decomposition

$$
d\mathbf x
=\mathbf e_r\,dr+r\mathbf e_\theta\,d\theta
+r\sin\theta\,\mathbf e_\phi\,d\phi,
$$

where

$$
\begin{aligned}
\mathbf e_r&=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta),\\
\mathbf e_\theta&=(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\\
\mathbf e_\phi&=(-\sin\phi,\cos\phi,0).
\end{aligned}
$$

Thus the [scale factors of orthogonal coordinates](../../../../../../scale-factors-of-orthogonal-coordinates.md) are

$$
\boxed{h_r=1,\qquad h_\theta=r,\qquad h_\phi=r\sin\theta}.
$$

Since the [total differential](../../../../../../total-differential.md) satisfies

$$
df=f_r\,dr+f_\theta\,d\theta+f_\phi\,d\phi
=d\mathbf x\cdot\nabla f,
$$

comparison of coefficients gives the [gradient](../../../../../../gradient.md)

$$
\boxed{
\nabla f
=\mathbf e_r\frac{\partial f}{\partial r}
+\mathbf e_\theta\frac1r\frac{\partial f}{\partial\theta}
+\mathbf e_\phi\frac1{r\sin\theta}\frac{\partial f}{\partial\phi}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9A](../../9a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
