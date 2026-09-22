<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) $H^2(\Omega)\hookrightarrow L^\infty(\Omega)$ in dimension three, combined with the preceding estimate, gives

$$
\boxed{\|u\|_\infty\le C\|f\|_2.}
$$

One direct justification of this embedding is a bounded [Sobolev extension operator](../../../../../../sobolev-extension-operator.md) into $H^2(\mathbb R^3)$, followed by Fourier inversion and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md): $\int_{\mathbb R^3}(1+|\xi|^2)^{-2}d\xi<\infty$ bounds the inverse Fourier integral by the $H^2$ [norm](../../../../../../norm.md).

For radial forcing, the preceding part makes $u=U(r)$ and $f=F(r)$. Set $a=1/2$, $b=2$ and $H(r)=\int_a^rs^2F(s)\,ds$. The radial equation gives $r^2U'(r)=C_0+H(r)$. Both zero boundary values imply

$$
C_0=-\frac{\int_a^br^{-2}H(r)\,dr}{\int_a^br^{-2}\,dr},\qquad |C_0|\le\|H\|_\infty.
$$

Moreover $\|H\|_\infty\le(\int_a^bs^2ds)^{1/2}(\int_a^bs^2|F|^2ds)^{1/2}\le C\|f\|_2$. Since $r\ge a$, this proves the [radial Poisson gradient estimate](../../../../../../radial-poisson-gradient-estimate.md):

$$
\boxed{\|\nabla u\|_\infty=\|U'\|_\infty\le C\|f\|_2\quad\text{for radial }f.}
$$

For a nonradial counterexample choose $x_0$ in the shell and a nonconstant $\varphi\in C_c^\infty(B(0,1))$. For sufficiently small $\varepsilon$, set $u_\varepsilon(x)=\varepsilon^{1/2}\varphi((x-x_0)/\varepsilon)$ and $f_\varepsilon=\Delta u_\varepsilon$. These are smooth with support away from the boundary. Scaling gives

$$
\boxed{\|f_\varepsilon\|_2=\|\Delta\varphi\|_2,\qquad\|\nabla u_\varepsilon\|_\infty=\varepsilon^{-1/2}\|\nabla\varphi\|_\infty\longrightarrow\infty.}
$$

Thus the [failure of L2-to-Linfinity Poisson gradient bounds in three dimensions](../../../../../../failure-of-l2-to-linfinity-poisson-gradient-bounds-in-three-dimensions.md) is explicit, despite the valid $H^2$ and value-supremum estimates.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
