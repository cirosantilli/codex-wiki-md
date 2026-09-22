<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Eliminate [pressure](../../../../../../pressure.md) by multiplying the radial equation by $k_z$ and subtracting $k_x$ times the vertical equation. For $k_z\ne0$, incompressibility gives $\tilde u_z=-(k_x/k_z)\tilde u_x$, and the pressure-free relation is $s(k_x^2+k_z^2)\tilde u_x/k_z=2\Omega k_z\tilde u_y$. Substitution in the azimuthal equation yields

$$
\boxed{s^2=\Omega^2\frac{2qk_xk_z-k_z^2}{k_x^2+k_z^2}=-\Omega^2\frac{k_z^2}{k^2}\left(1-2q\frac{k_x}{k_z}\right).}
$$

Thus the [vertical shear instability](../../../../../../vertical-shear-instability.md) occurs when $2qk_xk_z>k_z^2$, or $2q(k_x/k_z)>1$ for $k_z\ne0$. Otherwise the nonzero modes oscillate; equality is marginal in the exponential-growth sense. With $q>0$, growing disturbances have $k_x/k_z>1/(2q)$ and are strongly inclined in [wavevector](../../../../../../wavevector.md) space.

Put $R=k_x/k_z$. Maximizing $(2qR-1)/(1+R^2)$ gives $qR^2-R-q=0$. For $q>0$, the unstable maximizing root is

$$
R_{\max}=\frac{1+\sqrt{1+4q^2}}{2q},\qquad \boxed{s_{\max}=\Omega\sqrt{\frac{\sqrt{1+4q^2}-1}{2}}=\Omega q\,[1+O(q^2)].}
$$

More precisely its bracket is $1-q^2/2+O(q^4)$, and $R_{\max}\sim q^{-1}$. This is the [maximum growth rate of the vertical shear instability](../../../../../../maximum-growth-rate-of-the-vertical-shear-instability.md). For negative $q$, the maximum uses the corresponding negative root and is asymptotically $\Omega|q|$. At $q=0$ there is no exponentially growing mode. The undivided formula handles $k_z=0$: $s^2=0$, not an exponential instability; an allowed vertical velocity can instead force a secular azimuthal change. The excluded $\mathbf k=0$ is a spatially uniform disturbance and does not belong to the stipulated nonconstant one-phase family.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
