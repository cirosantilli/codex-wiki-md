<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [pressure tensor](../../../../../../pressure-tensor.md) has Cartesian components $p_{ab}=\int f(v_a-u_a)(v_b-u_b)\,d^3v$. With zero mean [velocity](../../../../../../velocity.md) and an isotropic [galactic distribution function](../../../../../../galactic-distribution-function.md), off-diagonal components vanish by reflection symmetry and diagonal components are equal by rotational symmetry. Therefore

$$
p_{ab}=p\delta_{ab},\qquad p=\frac13\int f|\mathbf v|^2\,d^3v=n\langle v_a^2\rangle.
$$

Here $p$ is a tracer number-weighted random-motion stress, rather than thermodynamic pressure per volume. Its tensor [divergence](../../../../../../divergence.md) is $(\operatorname{div}\mathbf p)_a=\partial_b(p\delta_{ab})=\partial_ap$. The time-independent, nonstreaming [Jeans equation](../../../../../../jeans-equation.md) consequently reduces to

$$
\boxed{\nabla p=n\nabla\psi.}
$$

The [gravitational acceleration](../../../../../../gravitational-acceleration.md) convention is $\nabla\psi$: this $\psi$ differs by a sign from the usual [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) $\Phi$.

Let $z$ measure distance along the [line of sight](../../../../../../line-of-sight.md). [Spherical density projection](../../../../../../spherical-density-projection.md) gives

$$
N(R)=\int_{-\infty}^{\infty}n(\sqrt{R^2+z^2})\,dz
=2\int_R^\infty\frac{n(r)r}{\sqrt{r^2-R^2}}\,dr.
$$

Because isotropy makes the local second [stellar velocity moment](../../../../../../stellar-velocity-moment.md) along every [line of sight](../../../../../../line-of-sight.md) equal to $p/n$, and because there is no streaming motion, the projected moment is

$$
N(R)\sigma^2(R)=\int_{-\infty}^{\infty}p(\sqrt{R^2+z^2})\,dz
=2\int_R^\infty\frac{p(r)r}{\sqrt{r^2-R^2}}\,dr.
$$

This is the forward relation for [isotropic stellar pressure deprojection](../../../../../../isotropic-stellar-pressure-deprojection.md).

Both inversions follow from one [Abel transform](../../../../../../abel-transform.md) calculation. Write $F(u)=N(\sqrt u)$ and $a(v)=n(\sqrt v)$, so $F(u)=\int_u^\infty a(v)(v-u)^{-1/2}\,dv$. Compose the transforms, using [Tonelli's theorem](../../../../../../tonelli-theorem.md) for nonnegative densities, or absolute convergence for signed profiles:

$$
\begin{aligned}
J(x)&=\int_x^\infty\frac{F(u)}{\sqrt{u-x}}\,du\\
&=\int_x^\infty a(v)\left[\int_x^v\frac{du}{\sqrt{(u-x)(v-u)}}\right]dv
=\pi\int_x^\infty a(v)\,dv.
\end{aligned}
$$

Assume sufficient decay to make these integrals finite and sufficient regularity for the last derivative. Then $J'(x)=-\pi a(x)$. Setting $x=r^2$ gives the [spherical Abel deprojection](../../../../../../spherical-abel-deprojection.md)

$$
\boxed{n(r)=-\frac1{2\pi r}\frac d{dr}\int_{r^2}^\infty\frac{N(\sqrt u)}{\sqrt{u-r^2}}\,du.}
$$

Replacing $F(u)$ by $N(\sqrt u)\sigma^2(\sqrt u)$ and $a(v)$ by $p(\sqrt v)$ proves

$$
\boxed{p(r)=-\frac1{2\pi r}\frac d{dr}\int_{r^2}^\infty\frac{N(\sqrt u)\sigma^2(\sqrt u)}{\sqrt{u-r^2}}\,du.}
$$

These are the requested expressions, with $u=R^2$. The composed-transform argument avoids an invalid separate differentiation of a divergent lower-end kernel.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
