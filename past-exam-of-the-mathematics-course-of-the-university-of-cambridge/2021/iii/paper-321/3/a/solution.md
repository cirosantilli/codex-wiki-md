<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md) velocity $\mathbf U=-(3/2)\Omega x\mathbf e_y$, its material acceleration vanishes because $\mathbf U\cdot\nabla\mathbf U=0$. The $x$ component of the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) is $-3\Omega^2x$, which is cancelled by $-\nabla\Phi_t=+3\Omega^2x\mathbf e_x$ with the signs in the stated equation; constant $P_0$ supplies no force. The flow is also incompressible.

Let $\mathbf u=\mathbf U+\mathbf u'$ and $h'=P'/\rho$. Axisymmetry removes $\mathbf U\cdot\nabla\mathbf u'$, while $\mathbf u'\cdot\nabla\mathbf U=-(3/2)\Omega u_x'\mathbf e_y$. Keeping first-order terms gives

$$
\boxed{\partial_tu_x'=-\partial_xh'+2\Omega u_y'},
\qquad
\boxed{\partial_tu_y'=-\frac12\Omega u_x'},
$$



$$
\boxed{\partial_tu_z'=-\partial_zh'},
\qquad
\boxed{\partial_xu_x'+\partial_zu_z'=0}.
$$

Differentiate the momentum equations in time and use incompressibility to eliminate $h'$. The radial velocity obeys

$$
\boxed{\partial_t^2(\nabla^2u_x')
+\Omega^2\partial_z^2u_x'=0}.
$$

For a plane wave proportional to $e^{i(k_xx+k_zz-\omega t)}$, this gives the [inertial wave](../../../../../../inertial-wave.md) dispersion relation

$$
\boxed{\omega^2=\Omega^2
\frac{k_z^2}{k_x^2+k_z^2}}.
$$

When $k_x=0$ and $k_z\ne0$, incompressibility forces $u_z'=0$, and the vertical momentum equation then forces $h'=0$. The remaining motion has $\omega=\pm\Omega$ and satisfies $u_y'=\mp i u_x'/2$: each horizontal layer executes an [epicyclic motion](../../../../../../epicyclic-motion.md), with the phase varying vertically but no pressure or vertical-velocity perturbation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
