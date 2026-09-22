<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [second-order rough-surface scattered field](../../../../../../second-order-rough-surface-scattered-field.md), the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) expanded at the mean plane is

$$
\psi_s^{[2]}(x,0)=-h\partial_z\psi_s^{[1]}(x,0)-\frac{h^2}{2}\partial_z^2\psi^{[0]}(x,0).
$$

At normal incidence, $\psi^{[0]}=e^{-ikz}-e^{ikz}$, so its second normal derivative vanishes at zero. Define the [Dirichlet-to-Neumann map for a Helmholtz half-space](../../../../../../dirichlet-to-neumann-map-for-a-helmholtz-half-space.md) through the [Fourier multiplier](../../../../../../fourier-multiplier.md) $\mathcal B$:

$$
\widehat{\mathcal B h}(q)=\beta(q)\widehat h(q),\qquad \partial_z\mathcal E g\big|_{z=0}=i\mathcal B g.
$$

The first-order trace is $2ikh$, hence $\partial_z\psi_s^{[1]}(x,0)=-2k\mathcal B h(x)$. It follows that

$$
\boxed{\psi_s(x,0)=-1+2ikh(x)+2k\,h(x)\mathcal B h(x)+O(\varepsilon^3),}
$$

where $h=O(\varepsilon)$ with fixed regular profile. In integral notation the quadratic contribution is

$$
2k\,h(x)\mathcal B h(x)=\frac{k}{\pi}h(x)\int\beta(q)\widehat h(q)e^{iqx}dq.
$$

The second-order field above the mean plane is $\mathcal E[2k h\mathcal B h]$ added to $-e^{ikz}+\mathcal E[2ikh]$. No local replacement of $\beta(q)$ by $k$ has been made; such a replacement would be an additional long-spatial-scale approximation.

The [physical surface trace and reference-plane trace](../../../../../../physical-surface-trace-and-reference-plane-trace.md) are distinct. At the actual rough boundary $z=h(x)$, the condition itself says $\psi_s(x,h(x))=-e^{-ikh(x)}$, so

$$
\boxed{\psi_s(x,h(x))=-1+ikh(x)+\frac{k^2h(x)^2}{2}+O(\varepsilon^3).}
$$

The first boxed expression is the reference-plane trace needed in part (d), at $z=0$, using the perturbative continuation where that plane lies below the actual boundary; the second answers the literal “at the surface” wording if it means the physical boundary. Taylor-expanding the first expression and its normal derivatives from $z=0$ to $z=h$ reproduces the second, so there is no contradiction between them.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
