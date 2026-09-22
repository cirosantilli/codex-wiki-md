<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [divergence of a Riemannian vector field](../../../../../divergence-of-a-riemannian-vector-field.md) $X$ is the trace of the [covariant derivative](../../../../../covariant-derivative.md) map $Y\mapsto\nabla_YX$:

$$
\operatorname{div}X=\sum_i g(\nabla_{e_i}X,e_i)
=\frac1{\sqrt{\det g}}\partial_i\bigl(\sqrt{\det g}\,X^i\bigr).
$$

It is characterized by $\mathcal L_X\omega_g=(\operatorname{div}X)\omega_g$ in the oriented case. The metric-dual vector field $X_\theta=\theta^\sharp$ is defined by $g(X_\theta,Y)=\theta(Y)$ for every $Y$, using the [musical isomorphism](../../../../../musical-isomorphism.md).

On a compact oriented manifold without boundary, the permitted exactness assertion and [Stokes theorem](../../../../../stokes-theorem.md) imply $\int_M\operatorname{div}Y\,\omega_g=0$ for every smooth vector field $Y$. For a smooth function $a$, the product rule gives

$$
\operatorname{div}(aX_\theta)=X_\theta(a)+a\operatorname{div}X_\theta.
$$

Since $\langle da,\theta\rangle=X_\theta(a)$, the formal-adjoint identity yields

$$
\int_M a\,\delta\theta\,\omega_g
=\int_M\langle da,\theta\rangle\omega_g
=-\int_M a\,\operatorname{div}X_\theta\,\omega_g.
$$

This holds for all $a$; taking $a=\delta\theta+\operatorname{div}X_\theta$ proves the pointwise formula

$$
\boxed{\delta\theta=-\operatorname{div}(\theta^\sharp)}.
$$

It agrees with $\delta\theta=-*d*\theta$, since $*\theta=\iota_{X_\theta}\omega_g$ and $d\iota_{X_\theta}\omega_g=\mathcal L_{X_\theta}\omega_g$.

The [Bochner formula for one-forms](../../../../../bochner-weitzenbock-formula-for-one-forms.md), with the positive [Hodge Laplacian](../../../../../hodge-laplacian.md), is

$$
\boxed{\Delta\theta=\nabla^*\nabla\theta+\operatorname{Ric}^{\sharp}\theta}.
$$

Here $\Delta=d\delta+\delta d$ acts on [one-forms](../../../../../one-form.md). The [covariant derivative](../../../../../covariant-derivative.md) $\nabla\theta$ is a section of $T^*M\otimes T^*M$, and its formal-adjoint composition, the [rough Laplacian](../../../../../rough-laplacian.md), is

$$
\nabla^*\nabla\theta=-\sum_i\left(\nabla_{e_i}\nabla_{e_i}\theta-\nabla_{\nabla_{e_i}e_i}\theta\right).
$$

This expression is independent of the local orthonormal frame. The Ricci term is the zero-order bundle endomorphism specified by

$$
(\operatorname{Ric}^{\sharp}\theta)(Y)=\operatorname{Ric}(\theta^\sharp,Y),\qquad
(\Delta\theta)_i=-\nabla^j\nabla_j\theta_i+\operatorname{Ric}_i{}^j\theta_j.
$$

Thus the identity separates the differential energy of the form from the curvature contribution; the sign of the Ricci term matches positive [sectional curvature](../../../../../sectional-curvature.md) on the sphere.

Let $\theta$ be a [harmonic one-form](../../../../../harmonic-one-form.md) on a compact connected manifold with nonnegative [Ricci curvature](../../../../../ricci-curvature.md). Pair the formula with $\theta$ and integrate:

$$
0=\int_M\langle\Delta\theta,\theta\rangle\,d\operatorname{vol}_g
=\int_M\left(|\nabla\theta|^2+\operatorname{Ric}(X_\theta,X_\theta)\right)d\operatorname{vol}_g.
$$

Both integrands are nonnegative and continuous, so each vanishes everywhere. In particular $\nabla\theta=0$, proving that [harmonic one-forms are parallel under nonnegative Ricci curvature](../../../../../harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature.md). This integration uses the Riemannian volume density and formal adjoints, so orientation is not necessary for the final conclusion.

Fix $p\in M$. The evaluation map

$$
\operatorname{ev}_p:\mathcal H^1(M)\longrightarrow T_p^*M,\qquad \theta\longmapsto\theta_p
$$

is injective: a parallel form with zero value at $p$ stays zero under [parallel transport](../../../../../parallel-transport.md) along every path, and connectedness makes every point reachable from $p$. Therefore

$$
\boxed{\dim\mathcal H^1(M)\le\dim T_p^*M=\dim M}.
$$

This is the [dimension bound for harmonic one-forms under nonnegative Ricci curvature](../../../../../dimension-bound-for-harmonic-one-forms-under-nonnegative-ricci-curvature.md). The bound is sharp: on a flat $n$-torus the $n$ constant coordinate [one-forms](../../../../../one-form.md) are parallel and harmonic. If [Ricci curvature](../../../../../ricci-curvature.md) is positive definite at even one point, the same integral and parallelism argument force every [harmonic one-form](../../../../../harmonic-one-form.md) to vanish.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
