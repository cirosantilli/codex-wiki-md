<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First take the spacetime trace of the generalized field equation. Since $n_\mu Z^\mu=-\Theta$ and spacetime has dimension four, this gives

$$
{}^{(4)}R+2\nabla_\mu Z^\mu-2\Theta=-8\pi T.
$$

Next contract twice with the unit normal. The result is

$$
R_{\mu\nu}n^\mu n^\nu
+2n^\mu n^\nu\nabla_\mu Z_\nu-\Theta
=8\pi\rho+4\pi T.
$$

Adding the trace equation to twice this normal projection cancels $T$. The [Scalar Gauss equation](../../../../../../scalar-gauss-equation.md) then converts the curvature terms to

$$
{}^{(3)}R+K^2-K_{\mu\nu}K^{\mu\nu}.
$$

For the derivative terms, part (iii) gives

$$
2\nabla_\mu Z^\mu+4n^\mu n^\nu\nabla_\mu Z_\nu
=2D^\mu Z_\mu+2n^\mu n^\nu\nabla_\mu Z_\nu.
$$

Differentiating $n^\nu Z_\nu=-\Theta$ along $n^\mu$ yields

$$
n^\mu n^\nu\nabla_\mu Z_\nu
=-n^\mu\nabla_\mu\Theta-Z_\nu a^\nu.
$$

Combining these identities produces

$$
\boxed{
{}^{(3)}R+K^2-K_{\mu\nu}K^{\mu\nu}
-2n^\mu\nabla_\mu\Theta-2Z_\mu a^\mu
-4\Theta+2D^\mu Z_\mu=16\pi\rho.
}
$$

Because $\Theta$ is a [scalar field](../../../../../../scalar-field.md) and $n^\mu=\alpha^{-1}(1,-\beta^i)$,

$$
n^\mu\nabla_\mu\Theta
=\frac1\alpha(\partial_t-\beta^m\partial_m)\Theta.
$$

The [normal acceleration](../../../../../../normal-acceleration.md) is spatial, so $Z_\mu a^\mu=\Theta_\mu a^\mu$. Part (iv) also gives $D^\mu Z_\mu=D^\mu\Theta_\mu-K\Theta$. Solving the preceding constraint for $\partial_t\Theta$ gives

$$
\partial_t\Theta=\beta^m\partial_m\Theta+\frac\alpha2
\left[
{}^{(3)}R+K(K-2\Theta)-K_{\mu\nu}K^{\mu\nu}
-2\Theta_\mu a^\mu-4\Theta
+2D^\mu\Theta_\mu-16\pi\rho
\right].
$$

Thus the constants in this [Z4 formulation](../../../../../../z4-formulation.md) evolution equation are

$$
\boxed{d_1=-2,\qquad d_2=-2,\qquad d_3=2,\qquad d_4=-16\pi.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 357](../../../paper-357-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
