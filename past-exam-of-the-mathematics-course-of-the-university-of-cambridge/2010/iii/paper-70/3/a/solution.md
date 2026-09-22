<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $e^{-i\omega t}$ time dependence and measure angles from the upward normal. Write $p_i=k\sin\theta_i$, $q_i=k\cos\theta_i>0$ and choose incident amplitude $A_i$. Separate the flat Dirichlet reflection from the rough correction:

$$
\psi^{[0]}=A_i e^{ip_ix-iq_iz}-A_i e^{ip_ix+iq_iz},\qquad
\psi=\psi^{[0]}+\psi_s^{[1]}+O(h^2).
$$

[Taylor expansion](../../../../../../taylor-expansion.md) of the boundary condition about $z=0$ gives

$$
0=\psi^{[0]}(x,0)+h(x)\partial_z\psi^{[0]}(x,0)+\psi_s^{[1]}(x,0)+O(h^2).
$$

Since $\partial_z\psi^{[0]}(x,0)=-2iq_iA_ie^{ip_ix}$, the induced trace is

$$
\boxed{\psi_s^{[1]}(x,0)=2iq_iA_ih(x)e^{ip_ix}.}
$$

Use $\widehat h(Q)=\int h(x)e^{-iQx}dx$ and $\beta(\xi)=\sqrt{k^2-\xi^2}$ with the outgoing branch: $\beta>0$ for $|\xi|<k$ and $\operatorname{Im}\beta>0$ outside. The [outgoing angular spectrum](../../../../../../outgoing-angular-spectrum.md) solves the [Helmholtz equation](../../../../../../helmholtz-equation.md) with that trace, giving the [first-order rough-surface scattered field](../../../../../../first-order-rough-surface-scattered-field.md)

$$
\boxed{\psi_s^{[1]}(x,z)=\frac{iq_iA_i}{\pi}\int_{\mathbb R}\widehat h(\xi-p_i)e^{i\xi x+i\beta(\xi)z}d\xi.}
$$

If “[scattered field](../../../../../../scattered-wave.md)” includes the specular reflection, add $-A_i e^{ip_ix+iq_iz}$ to this rough correction. [Fourier transforms](../../../../../../fourier-transform.md) of an infinite random surface are generalized objects; finite-window transforms give an ordinary [integral](../../../../../../integral.md) and are also needed for its far-field intensity. The expansion assumes a fixed regular surface shape scaled to small height. Highly oscillatory profiles can require additional control of slopes and spectral moments; small height alone is not a uniform error estimate for every profile.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
