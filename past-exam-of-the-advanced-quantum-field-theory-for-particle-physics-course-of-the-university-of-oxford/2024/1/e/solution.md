<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Collect the two [Dirac fields](../../../../dirac-field.md) into $\Psi=(\psi_1,\psi_2)^T$, with a common nonzero [mass](../../../../mass.md) $m$. Then

$$
\boxed{\mathcal L=\sum_{i=1}^2\bar\psi_i(i\not\partial-m)\psi_i
=\bar\Psi(i\not\partial-m\mathbf1_2)\Psi.}
$$

Among complex-linear rotations of the [Dirac fields](../../../../dirac-field.md), the [internal symmetry of a classical field theory](../../../../internal-symmetry-of-a-classical-field-theory.md) is $\Psi\mapsto U\Psi$, $U\in U(2)$, with $\bar\Psi\mapsto\bar\Psi U^\dagger$. Unitarity preserves the kinetic term, and the [mass matrix](../../../../mass-matrix.md) commutes with every $U$. This [unitary flavour symmetry of degenerate Dirac fields](../../../../unitary-flavour-symmetry-of-degenerate-dirac-fields.md) has [group](../../../../group-split.md) $(SU(2)\times U(1))/\mathbb Z_2$, where the quotient avoids counting the common central element twice.

Choose the four [Hermitian matrices](../../../../hermitian-operator.md) $T^0=\mathbf1_2/2$, $T^a=\sigma^a/2$ for $a=1,2,3$, with $\sigma^a$ the [Pauli matrices](../../../../pauli-matrices.md). Promoting the four parameters to functions gives $\delta S=-\int d^4x\,(\partial_\mu\alpha^A)\bar\Psi\gamma^\mu T^A\Psi$. The four [Noether currents](../../../../noether-current.md) are therefore

$$
\boxed{j_A^\mu=\bar\Psi\gamma^\mu T^A\Psi,\qquad A=0,1,2,3.}
$$

Their divergences vanish by the equal-mass [Dirac equations](../../../../dirac-equation.md). The singlet is half the total [Dirac current](../../../../dirac-current.md); the other three currents rotate the two species.

**Free-theory qualification.** If “global internal symmetry” allows mixing the [Dirac fields](../../../../dirac-field.md) with [charge-conjugate fields](../../../../charge-conjugate-field.md), the completely free theory written here has a larger [enhanced internal symmetry of free Dirac fields](../../../../enhanced-internal-symmetry-of-free-dirac-fields.md). Write $\psi_i=(\lambda_{2i-1}+i\lambda_{2i})/\sqrt2$ using four [Majorana fermions](../../../../majorana-spinor.md). Up to a [total derivative](../../../../total-derivative.md),

$$
\mathcal L=\frac12\sum_{A=1}^4\bar\lambda_A(i\not\partial-m)\lambda_A.
$$

The full [orthogonal group](../../../../orthogonal-group.md) $O(4)$ acts on the four real species; its connected part is $SO(4)$. Its six [Noether currents](../../../../noether-current.md) can be chosen as $J_{AB}^\mu=i\bar\lambda_A\gamma^\mu\lambda_B$ for $A<B$, up to the common sign convention. The antisymmetry of this [Majorana fermion](../../../../majorana-spinor.md) vector bilinear makes these the six independent rotations. A concrete rotation outside the stated complex-linear $U(2)$ is $\lambda_2\mapsto\cos\theta\lambda_2+\sin\theta\lambda_3$, $\lambda_3\mapsto-\sin\theta\lambda_2+\cos\theta\lambda_3$: it preserves the displayed [Lagrangian density](../../../../lagrangian-density.md) while mixing $\psi_i$ with their [charge-conjugate fields](../../../../charge-conjugate-field.md). The usual $U(2)$ answer specifies the subgroup preserving the chosen common [fermion number](../../../../fermion-number.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
