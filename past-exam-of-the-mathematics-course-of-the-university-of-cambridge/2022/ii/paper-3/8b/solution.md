<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

The [generalized momenta](../../../../../generalized-momentum.md) conjugate to the two [ignorable coordinates](../../../../../ignorable-coordinate.md) are

$$
\boxed{
p_\phi
=I_1\dot\phi\sin^2\theta
+I_3(\dot\psi+\dot\phi\cos\theta)\cos\theta
}
$$

and

$$
\boxed{
p_\psi=I_3(\dot\psi+\dot\phi\cos\theta)
}.
$$

Since the Lagrangian contains neither $\phi$ nor $\psi$, both momenta are constant in time.

Eliminating the two angular velocities gives

$$
\dot\phi=\frac{p_\phi-p_\psi\cos\theta}
{I_1\sin^2\theta},
\qquad
\dot\psi+\dot\phi\cos\theta=\frac{p_\psi}{I_3}.
$$

Conservation of energy then yields the [heavy symmetric top reduction](../../../../../heavy-symmetric-top-reduction.md)

$$
\frac12I_1\dot\theta^2+V_{\rm eff}(\theta)=E,
$$

where

$$
\boxed{
V_{\rm eff}(\theta)
=\frac{(p_\phi-p_\psi\cos\theta)^2}
{2I_1\sin^2\theta}
+\frac{p_\psi^2}{2I_3}
+Mgl\cos\theta
}.
$$

As $\theta\to0$, the first term diverges unless

$$
\boxed{p_\phi=p_\psi}.
$$

Writing their common value as $p$, the small-angle expansion is

$$
V_{\rm eff}(\theta)
=\frac{p^2}{2I_3}+Mgl
+\left(\frac{p^2}{8I_1}-\frac{Mgl}{2}\right)\theta^2
+O(\theta^4).
$$

By the [effective potential stability criterion](../../../../../effective-potential-stability-criterion.md), the vertical state is stable exactly when

$$
\boxed{p^2>4I_1Mgl}.
$$

At the vertical state $p=I_3(\dot\psi+\dot\phi)$, so this is the [gyroscopic stabilization of an inverted symmetric top](../../../../../gyroscopic-stabilization-of-an-inverted-symmetric-top.md) by sufficiently rapid spin.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
