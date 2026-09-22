<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Vary the action with compactly supported variations and integrate by parts. Its overall normalization does not affect the equation of motion:

$$
\partial_\mu(\sqrt{-g}\,g^{\mu\nu}\partial_\nu\phi)=0.
$$

Here $\sqrt{-g}=e^{3t}$, so the [massless scalar field](../../../../../../massless-scalar-field.md) obeys

$$
\phi_{tt}+3\phi_t-e^{-2t}\nabla^2\phi=0.
$$

Separate a spatial [Fourier mode](../../../../../../fourier-mode.md) as $\phi(t,\mathbf x)=F_k(t)e^{i\mathbf k\cdot\mathbf x}$. Its mode equation is $F_{k,tt}+3F_{k,t}+k^2e^{-2t}F_k=0$. With [conformal time](../../../../../../conformal-time.md) $\tau=-e^{-t}$, $a=-1/\tau$ and $\mathcal H=-1/\tau$, it becomes

$$
F_k''-\frac2\tau F_k'+k^2F_k=0.
$$

For $k>0$, put $z=-k\tau=ke^{-t}$ and $F_k=z^2G(z)$. Direct differentiation reduces the equation to

$$
G_{zz}+\frac2zG_z+\left(1-\frac2{z^2}\right)G=0,
$$

the [Spherical Bessel function](../../../../../../spherical-bessel-function.md) equation with order one. Hence the complete classical mode basis is

$$
\boxed{F_k(t)=z^2[C_{\mathbf k}j_1(z)+D_{\mathbf k}y_1(z)],\qquad z=ke^{-t}.}
$$

Since $z^2j_1(z)=\sin z-z\cos z$ and $z^2y_1(z)=-\cos z-z\sin z$, an equivalent complex basis is

$$
\boxed{F_k(\tau)=A_{\mathbf k}(1+ik\tau)e^{-ik\tau}
+B_{\mathbf k}(1-ik\tau)e^{ik\tau}.}
$$

The classical action does not select one frequency branch or a quantum vacuum. A real field has conjugate-related coefficients at opposite wavevectors. The zero mode, which is not obtained by treating these two $k>0$ basis functions as independent at $k=0$, is

$$
\boxed{F_0(t)=C_0+D_0e^{-3t}.}
$$

At late times one independent solution freezes and the other decays as $e^{-3t}$. These are minimally coupled massless modes; the supplied action has no curvature-coupling term, so it should not be replaced by the conformally coupled wave equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
