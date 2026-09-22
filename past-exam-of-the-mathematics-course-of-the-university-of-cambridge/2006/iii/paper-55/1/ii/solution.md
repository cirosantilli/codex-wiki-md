<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Separate background [stress-energy conservation](../../../../../../stress-energy-conservation.md) gives $\rho_C'=-3\mathcal H\rho_C$ and $\rho_S'=-2\mathcal H\rho_S$. Therefore

$$
\rho_C\propto a^{-3},\quad \rho_S\propto a^{-2},\quad
\eta=\frac{\rho_S}{\rho_C}\propto a,\quad
\eta'=\mathcal H\eta,\quad \Omega_C=\frac1{1+\eta}.
$$

For consistency, compute the expansion derivative from the [Friedmann equation](../../../../../../friedmann-equations.md), rather than assume the printed second hint. Differentiating $\mathcal H^2=(8\pi G/3)a^2\rho_{\rm tot}$ and using total [stress-energy conservation](../../../../../../stress-energy-conservation.md) yields

$$
\mathcal H'=-\frac{4\pi G}{3}a^2(\rho_{\rm tot}+3P_{\rm tot})
=-\frac{4\pi G}{3}a^2\rho_C
=-\frac{\mathcal H^2}{2(1+\eta)}.
$$

The PDF's hint has $\rho_{\rm tot}+P_{\rm tot}$ where $\rho_{\rm tot}+3P_{\rm tot}$ is required. It is incompatible with the first hint and conservation, and would not give the requested equation. The expression above is the corrected conformal-time acceleration identity.

For a function $D(\eta)=\delta_C$, the chain rule gives

$$
\delta_C'=\mathcal H\eta D_\eta,\qquad
\delta_C''=\mathcal H^2\eta^2D_{\eta\eta}
+\eta(\mathcal H'+\mathcal H^2)D_\eta.
$$

Substituting in the cold-matter equation and dividing by $\mathcal H^2\eta^2$ produces

$$
D_{\eta\eta}+\frac{2+\mathcal H'/\mathcal H^2}{\eta}D_\eta
-\frac{3}{2\eta^2(1+\eta)}D=0,
$$

or

$$
\boxed{D_{\eta\eta}+\frac{3+4\eta}{2\eta(1+\eta)}D_\eta
-\frac{3D}{2\eta^2(1+\eta)}=0.}
$$

This is [cold-matter growth in a matter-coasting-fluid universe](../../../../../../cold-matter-growth-in-a-matter-coasting-fluid-universe.md); its coefficients depend on the background density ratio, not on $k$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
