<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Before recombination, tight coupling makes photons and baryons share an adiabatic perturbation. Since $\delta\rho_b/\rho_b=(3/4)\delta\rho_r/\rho_r$ and only radiation supplies appreciable pressure,

$$
\delta P=\frac{c^2}{3}\delta\rho_r,\qquad
\delta\rho=\delta\rho_r\left(1+\frac{3\rho_b}{4\rho_r}\right).
$$

Thus the [photon-baryon sound speed](../../../../../../photon-baryon-sound-speed.md) is

$$
\boxed{c_s=\frac c{\sqrt3}\left(1+\frac{3\rho_b}{4\rho_r}\right)^{-1/2}}.
$$

Because $\rho_r\propto a^{-4}$ and $\rho_b\propto a^{-3}$,

$$
c_s\propto
\begin{cases}
a^0,&t<t_{\rm eq},\\
a^{-1/2},&t_{\rm eq}<t<t_{\rm rec}.
\end{cases}
$$

After [cosmological recombination](../../../../../../recombination-cosmology.md), baryons decouple from radiation; for adiabatically cooling nonrelativistic gas, $T_b\propto a^{-2}$ and $c_s\propto a^{-1}$.

The [comoving Jeans length](../../../../../../comoving-jeans-length.md) is

$$
\lambda_{\rm com}=\frac{c_s}{a}\sqrt{\frac{\pi}{G\bar\rho}}.
$$

During radiation domination $\bar\rho\propto a^{-4}$, so $\lambda_{\rm com}\propto a$. During matter domination before recombination, $\bar\rho\propto a^{-3}$ and $c_s\propto a^{-1/2}$, so $\lambda_{\rm com}$ is approximately constant. Recombination causes a sharp downward jump in sound speed, after which $\lambda_{\rm com}\propto a^{-1/2}$. The requested log-log sketch therefore rises with slope one, reaches a plateau after equality, drops at recombination, and then declines with slope $-1/2$.

For collisionless particles, replace $c_s$ by their one-dimensional velocity dispersion $v_{\rm rms}$:

$$
\boxed{\lambda_{\rm com}^{\rm coll}
=\frac{v_{\rm rms}}a\sqrt{\frac{\pi}{G\bar\rho}}}.
$$

For a thermally produced cold relic, identify four epochs:

- while coupled and relativistic, $v_{\rm rms}\simeq c$ and $\lambda_{\rm com}\propto a$ in radiation domination;
- after decoupling but while still relativistic, momentum redshifts but speed remains near $c$, so the same $\lambda_{\rm com}\propto a$ scaling continues with collisionless free streaming;
- after becoming nonrelativistic but before equality, $v_{\rm rms}\propto a^{-1}$ and $\bar\rho\propto a^{-4}$, giving $\lambda_{\rm com}\propto a^0$;
- after equality, $v_{\rm rms}\propto a^{-1}$ and $\bar\rho\propto a^{-3}$, giving $\lambda_{\rm com}\propto a^{-1/2}$.

Its plot rises through the two relativistic epochs, turns onto a plateau at the nonrelativistic transition, and falls after equality. Recombination does not dynamically affect collisionless dark matter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
