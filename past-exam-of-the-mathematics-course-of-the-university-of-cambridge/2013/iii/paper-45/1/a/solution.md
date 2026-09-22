<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take real field coordinates $\phi^I$; for complex [scalar fields](../../../../../../scalar-field.md), split them into real and imaginary parts. Assume a smooth [scalar potential](../../../../../../scalar-potential.md) and positive, canonically normalized [kinetic terms](../../../../../../kinetic-term.md) in a relativistic theory. At a [classical vacuum](../../../../../../classical-vacuum.md), $V_I(\phi_0)=0$. The [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
V(\phi_0+\xi)=V(\phi_0)+\frac12\xi^I(M^2)_{IJ}\xi^J+O(\|\xi\|^3),\qquad (M^2)_{IJ}=\left.\frac{\partial^2 V}{\partial\phi^I\partial\phi^J}\right|_{\phi_0}.
$$

Thus the [scalar mass matrix](../../../../../../scalar-mass-matrix.md) is the [Hessian matrix](../../../../../../hessian-matrix.md), and its [eigenvalues](../../../../../../eigenvalue.md) give squared masses of the linearized scalar excitations.

Put $X_a(\phi)=it^a\phi$. Infinitesimal invariance of the [scalar potential](../../../../../../scalar-potential.md) gives the identity $V_I X_a^I=0$ at every field value. Differentiate with respect to $\phi^J$ and evaluate at the [classical vacuum](../../../../../../classical-vacuum.md):

$$
(M^2)_{JI}X_a^I(\phi_0)+V_I(\phi_0)\partial_JX_a^I(\phi_0)=0,
\qquad\boxed{M^2(it^a\phi_0)=0.}
$$

Every nonzero infinitesimal symmetry direction therefore lies in the [kernel](../../../../../../kernel-of-a-linear-map.md) of the [scalar mass matrix](../../../../../../scalar-mass-matrix.md). This is the classical [Goldstone theorem](../../../../../../goldstone-theorem.md) expressed through [Goldstone directions in the scalar mass matrix](../../../../../../goldstone-directions-in-the-scalar-mass-matrix.md).

Let $H_0$ be the full [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) of $\phi_0$. The linear map from the [Lie algebra](../../../../../../lie-algebra-split.md) of $G$ to field space, $T\mapsto iT\phi_0$, has kernel equal to the [Lie algebra](../../../../../../lie-algebra-split.md) of $H_0$. The [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) gives

$$
\boxed{\dim\operatorname{span}\{it^a\phi_0\}=\dim G-\dim H_0.}
$$

There are consequently **at least $\dim G-\dim H_0$ massless scalar directions**, namely the tangent directions to the symmetry orbit through the [classical vacuum](../../../../../../classical-vacuum.md). If the intended $H$ is $H_0$, these are the $\dim G-\dim H$ symmetry-required [Goldstone bosons](../../../../../../goldstone-boson.md). Exactly that many massless modes occur if the [scalar mass matrix](../../../../../../scalar-mass-matrix.md) is positive definite on a complement of those tangent directions. A nonsingular positive field-space kinetic metric changes normalization, but not the number of zero masses.

Two qualifications are needed for the literal assumptions. A subgroup fixing the [classical vacuum](../../../../../../classical-vacuum.md) need not be the full [stabilizer subgroup](../../../../../../stabilizer-subgroup.md). For example, take $G=SO(3)$ acting on a real triplet and $V=\lambda(|\phi|^2-v^2)^2/8$ with $\lambda,v>0$. At $\phi_0=ve_3$, the [scalar mass matrix](../../../../../../scalar-mass-matrix.md) is $\lambda v^2\operatorname{diag}(0,0,1)$: there are two massless modes. Choosing $H=\{1\}$ satisfies the printed invariance condition but would incorrectly predict three. The full [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) is $SO(2)$.

Even with the full [stabilizer subgroup](../../../../../../stabilizer-subgroup.md), symmetry does not exclude an [accidental massless scalar](../../../../../../accidental-massless-scalar.md). Take $G=SO(2)$ rotating $(x,y)$, with an invariant singlet $z$, and

$$
V(x,y,z)=\frac\lambda4(x^2+y^2-v^2)^2+\kappa z^4,\qquad\lambda,\kappa>0.
$$

At $(v,0,0)$ the full continuous stabilizer is trivial, but the [scalar mass matrix](../../../../../../scalar-mass-matrix.md) is $\operatorname{diag}(2\lambda v^2,0,0)$. One zero direction is the [Goldstone boson](../../../../../../goldstone-boson.md); the other is an [accidental massless scalar](../../../../../../accidental-massless-scalar.md) at quadratic order. **The proof establishes the symmetry-required count, not unconditional equality with the total number of massless fields.** The statement concerns global internal symmetry; gauging it changes the physical interpretation through the [Higgs mechanism](../../../../../../higgs-mechanism.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
