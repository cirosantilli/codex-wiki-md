<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The spatial metric is stationary and only $\beta^r=b(r)=Mr/(r+M)^2$ is nonzero. The evolution equation therefore says

$$
2\alpha K_{ij}=(\mathcal L_\beta\gamma)_{ij},
$$

the [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) of the spatial metric along the [shift vector](../../../../../../shift-vector.md). For the radial component,

$$
2\alpha K_{rr}
=b\,\partial_r\gamma_{rr}
+2\gamma_{rr}\partial_rb
=-\frac{2M}{r(r+M)},
$$

so

$$
\boxed{K_{rr}=-\frac{M}{r^2}.}
$$

For the angular components,

$$
2\alpha K_{\theta\theta}
=b\,\partial_r(r+M)^2
=\frac{2Mr}{r+M},
$$

and spherical symmetry supplies

$$
\boxed{
K_{\theta\theta}=M,\qquad
K_{\phi\phi}=M\sin^2\theta.
}
$$

All off-diagonal components vanish.

Contracting with the inverse spatial metric gives the [mean curvature](../../../../../../mean-curvature.md)

$$
\begin{aligned}
K&=\gamma^{rr}K_{rr}
+\gamma^{\theta\theta}K_{\theta\theta}
+\gamma^{\phi\phi}K_{\phi\phi}\\
&=-\frac{M}{(r+M)^2}
+\frac{M}{(r+M)^2}
+\frac{M}{(r+M)^2}.
\end{aligned}
$$

Thus

$$
\boxed{K=\frac{M}{(r+M)^2}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 357](../../../paper-357-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
