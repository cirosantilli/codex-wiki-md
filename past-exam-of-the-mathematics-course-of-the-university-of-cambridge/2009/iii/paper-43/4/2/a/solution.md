<h1 id="4/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $S=H/T$ and take $n\geq2$. The unit-length constraint prevents an arbitrary multiplicative field rescaling, so the running coupling is found by renormalizing the coefficient of $|\nabla\sigma|^2$. We compute that coefficient in a slowly rotating planar background, which is enough because $O(n)$ symmetry makes the two-derivative stiffness isotropic on the sphere.

Let $n_0=(\cos\theta,\sin\theta,0,\ldots)$, $e_1=(-\sin\theta,\cos\theta,0,\ldots)$ and $e_a$ for $2\leq a\leq n-1$ the remaining constant orthonormal tangent vectors. Parameterize the fast tangent fluctuations by

$$
\sigma=n_0q+\sum_{a=1}^{n-1}e_a\pi_a,\qquad q=\sqrt{1-\pi^2},\qquad \pi^2=\sum_a\pi_a^2.
$$

This satisfies $\sigma^2=1$ exactly. Put $\Omega_\mu=\partial_\mu\theta$, and choose it locally constant and small compared with the shell momenta. Since $\partial_\mu n_0=e_1\Omega_\mu$ and $\partial_\mu e_1=-n_0\Omega_\mu$, direct differentiation gives

$$
|\partial_\mu\sigma|^2=|\partial_\mu\pi|^2+(\partial_\mu q)^2
+\Omega_\mu^2\left(1-\sum_{a=2}^{n-1}\pi_a^2\right)
+2\Omega_\mu(q\partial_\mu\pi_1-\pi_1\partial_\mu q).
$$

At quadratic order in the fast fields, the cross term is $2\Omega_\mu\partial_\mu\pi_1$, whose integral is zero for constant $\Omega_\mu$. The term $(\partial q)^2$ is quartic in the fast fields. Remaining cross terms are cubic and have zero Gaussian expectation; their effects on the two-derivative stiffness start at higher loop order. Field-measure corrections independent of the background contribute normalization terms and do not alter the leading gradient coefficient in this calculation.

The quadratic fast action is $(2g)^{-1}\int|\nabla\pi|^2$. In the shell $\Lambda/b<|p|<\Lambda$ its [connected correlation function](../../../../../../../connected-correlation-function.md) is $\langle\pi_a(p)\pi_b(-p)\rangle=g\delta_{ab}/p^2$ with the momentum delta function understood. Thus $\langle\pi_a(x)^2\rangle=gI_D$, where

$$
I_D(b)=\int_{\Lambda/b<|p|<\Lambda}\frac{d^Dp}{(2\pi)^D}\frac1{p^2}
=\frac{S_D}{(2\pi)^D}\Lambda^\epsilon\frac{1-b^{-\epsilon}}{\epsilon},\qquad D=2+\epsilon,
$$

with the limit $I_2(b)=(2\pi)^{-1}\log b$. Here $S_D=2\pi^{D/2}/\Gamma(D/2)$ is the angular measure of the unit $(D-1)$-sphere. Averaging the background-gradient coefficient gives the [one-loop stiffness of a spherical nonlinear sigma model](../../../../../../../one-loop-stiffness-of-a-spherical-nonlinear-sigma-model.md):

$$
\frac1{g_{\rm eff}}=\frac1g\left[1-(n-2)gI_D\right]
=\frac1g-(n-2)I_D.
$$

The coefficient is $n-2$, not $n-1$: the fluctuation tangent to the rotation plane does not reduce the gradient cost, because its contribution cancels between $q^2$ and $\pi_1^2$. All other $n-2$ transverse components do reduce it.

After integrating out the shell, put $x=bx'$ to restore the cutoff. The constrained field keeps unit norm, so $g'=b^{-\epsilon}g_{\rm eff}$, or at this order

$$
g'=b^{-\epsilon}\left[g+(n-2)g^2 I_D(b)+O(g^3)\right].
$$

For $b=e^{d\ell}$, $I_D=(S_D/(2\pi)^D)\Lambda^\epsilon d\ell+O(d\ell^2)$. Therefore the [renormalization-group beta function](../../../../../../../beta-function-physics.md) is

$$
\boxed{\frac{dg}{d\log b}=-\epsilon g+\frac{S_D}{(2\pi)^D}\Lambda^\epsilon(n-2)g^2+O(g^3).}
$$

The displayed terms are the requested one-loop flow. They are a weak-coupling expansion; the discrete $n=1$ target has no tangent modes and must instead be treated by domain walls, as in the first part.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
