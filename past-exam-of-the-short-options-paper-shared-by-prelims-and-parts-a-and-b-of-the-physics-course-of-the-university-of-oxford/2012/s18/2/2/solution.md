<h1 id="s18/2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The spherical potential has a rotationally symmetric [Fourier transform](../../../../../fourier-transform-split.md), so choose the polar axis of the integration along $\mathbf q$. With $q=|\mathbf k_f-\mathbf k_i|=2k\sin(\theta/2)$,

$$
\int_{r'\le r_0}d^3\mathbf r'\,V_0e^{-i\mathbf q\cdot\mathbf r'}
=4\pi V_0\int_0^{r_0}r'^2\frac{\sin(qr')}{qr'}\,dr'
=4\pi V_0\frac{\sin(qr_0)-qr_0\cos(qr_0)}{q^3}.
$$

The [first Born approximation](../../../../../born-approximation.md) therefore gives

$$
\boxed{f_k(\theta)=-\frac{2mV_0}{\hbar^2q^3}\left[\sin(qr_0)-qr_0\cos(qr_0)\right],\qquad q=2k\sin\frac\theta2.}
$$

There is no azimuthal dependence. At $q=0$, the bracket is $(qr_0)^3/3+O(q^5)$, so $f_k(0)=-2mV_0r_0^3/(3\hbar^2)$ is finite, not zero. The approximation assumes scattering weak enough for the incident plane wave to replace the distorted wave inside the interaction integral.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [2](../../2.md)
3. [S18](../../../s18.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
