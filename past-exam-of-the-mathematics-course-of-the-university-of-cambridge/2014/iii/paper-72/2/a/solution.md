<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work above the surface, with $e^{-i\omega t}$ time dependence. Define the [scattered field](../../../../../../scattered-wave.md) by $\psi=\psi_i+\psi_s$, so it includes the reflection from a flat surface. For [small-height Dirichlet scattering](../../../../../../small-height-dirichlet-scattering.md), write $h=\varepsilon\eta$ and expand

$$
\psi_s=\psi_s^{[0]}+\psi_s^{[1]}+O(\varepsilon^2).
$$

The zeroth-order total field $\psi^{[0]}=\psi_i+\psi_s^{[0]}$ satisfies the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) $\psi^{[0]}(x,0)=0$. Taylor expansion at the perturbed boundary gives

$$
0=\psi^{[0]}(x,0)+h(x)\partial_z\psi^{[0]}(x,0)+\psi_s^{[1]}(x,0)+O(\varepsilon^2).
$$

Thus the [first-order rough-surface scattered field](../../../../../../first-order-rough-surface-scattered-field.md) has mean-plane boundary data $g_1(x)=-h(x)\partial_z\psi^{[0]}(x,0)$.

Use the [outgoing angular spectrum](../../../../../../outgoing-angular-spectrum.md) to solve this boundary-value problem. For $\widehat g(q)=\int g(x)e^{-iqx}dx$, let

$$
\beta(q)=\begin{cases}\sqrt{k^2-q^2},&|q|\leq k,\\i\sqrt{q^2-k^2},&|q|>k,\end{cases}\qquad (\mathcal E g)(x,z)=\frac1{2\pi}\int\widehat g(q)e^{iqx+i\beta(q)z}dq.
$$

The branch ensures upward propagation or upward evanescent decay. Each component solves the [Helmholtz equation](../../../../../../helmholtz-equation.md), and $\mathcal E g$ has trace $g$ at $z=0$. Consequently

$$
\boxed{\psi_s^{[0]}=-\mathcal E[\psi_i(\cdot,0)],\qquad \psi_s^{[1]}=-\mathcal E[h\,\partial_z\psi^{[0]}(\cdot,0)].}
$$

This gives the [scattered field](../../../../../../scattered-wave.md) through first order by adding the two contributions. If one reserves “rough [scattered field](../../../../../../scattered-wave.md)” for the non-specular correction, it is $\psi_s^{[1]}$ alone; the convention here keeps the flat reflection as well.

The expansion is in height for a fixed sufficiently regular profile. The condition $|kh|\ll1$ controls the [incident wave](../../../../../../incident-wave.md)'s height expansion, but very short spatial scales can create large evanescent normal derivatives. The surface regularity and relevant spectral moments must also control the subsequent boundary expansions; small [amplitude](../../../../../../wave-amplitude.md) alone is not a uniform guarantee for arbitrarily fine roughness.

## ↑ Ancestors (11)

1. [A](../a.md)
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
