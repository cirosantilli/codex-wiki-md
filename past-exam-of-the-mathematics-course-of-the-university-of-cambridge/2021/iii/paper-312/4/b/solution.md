<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the total derivative of the [phase-space distribution function](../../../../../../phase-space-distribution-function.md) as

$$
\frac{df}{d\eta}=\frac{\partial f}{\partial\eta}
+\frac{dx^i}{d\eta}\frac{\partial f}{\partial x^i}
+\frac{d\ln\epsilon}{d\eta}\frac{\partial f}{\partial\ln\epsilon}
+\frac{d\widehat p^i}{d\eta}\frac{\partial f}{\partial\widehat p^i}.
$$

Since $a\bar T$ is constant for the background photon gas, expand the [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md) as

$$
f=\bar f(\epsilon)-\epsilon\bar f_{,\epsilon}\Theta+O(2).
$$

At first order the four terms are respectively

$$
-\epsilon\bar f_{,\epsilon}\Theta',
\qquad
-\epsilon\bar f_{,\epsilon}\widehat p^i\partial_i\Theta,
\qquad
\epsilon\bar f_{,\epsilon}
(\Phi'-\widehat p^i\partial_i\Psi),
\qquad
0.
$$

The angular-deflection velocity is already first order and multiplies the first-order angular dependence of $f$, so its contribution is second order. Thus the collisionless left-hand side of the [Free-streaming photon Boltzmann equation](../../../../../../free-streaming-photon-boltzmann-equation.md) is

$$
\boxed{\frac{df}{d\eta}
=-\epsilon\bar f_{,\epsilon}
\left[\Theta'+\widehat{\mathbf p}\cdot\nabla\Theta
+\widehat{\mathbf p}\cdot\nabla\Psi-\Phi'\right]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
