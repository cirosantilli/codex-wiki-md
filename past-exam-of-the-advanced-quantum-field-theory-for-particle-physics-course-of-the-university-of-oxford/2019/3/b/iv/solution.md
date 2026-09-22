<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $H=\phi_1$ and $P=\phi_2$, both [Hermitian matrices](../../../../../hermitian-operator.md). Through quadratic order around the chosen [vacuum expectation value](../../../../../vacuum-expectation-value.md),

$$
X=\Phi^\dagger\Phi=C^2\mathbf1+\sqrt2 CH+\frac12(H^2+P^2+i[H,P]).
$$

The [trace of a commutator](../../../../../trace-of-a-commutator.md) vanishes. The needed [matrix traces](../../../../../matrix-trace.md) are therefore

$$
\begin{aligned}
\operatorname{tr}X&=NC^2+\sqrt2 C\operatorname{tr}H+\frac12\operatorname{tr}(H^2+P^2),\\
\operatorname{tr}X^2&=NC^4+2\sqrt2 C^3\operatorname{tr}H+C^2\operatorname{tr}(3H^2+P^2)+O((H,P)^3),\\
(\operatorname{tr}X)^2&=N^2C^4+2\sqrt2 NC^3\operatorname{tr}H+NC^2\operatorname{tr}(H^2+P^2)+2C^2(\operatorname{tr}H)^2+O((H,P)^3).
\end{aligned}
$$

Using $m^2=-(\alpha+N\beta)C^2$, all linear terms cancel. The quadratic [scalar potential](../../../../../scalar-potential.md) reduces to

$$
\boxed{V^{(2)}=\alpha C^2\operatorname{tr}H^2+\beta C^2(\operatorname{tr}H)^2,}
$$

with no $P^2$ term. The kinetic term is

$$
\mathcal L_{\mathrm{kin}}^{(2)}=\frac12\operatorname{tr}[(\partial H)^2+(\partial P)^2],
$$

since its mixed term is the [trace of a commutator](../../../../../trace-of-a-commutator.md). A [Hermitian matrix](../../../../../hermitian-operator.md) has $N^2$ independent real components, so $P$ describes exactly $N^2$ massless scalar modes.

To determine the other [masses](../../../../../mass.md), take $T_0=\mathbf1/\sqrt N$ and traceless Hermitian $T_A$ with $\operatorname{tr}(T_AT_B)=\delta_{AB}$, and expand $H=h_0T_0+\sum_{A=1}^{N^2-1}h_AT_A$. These are canonically normalized real [scalar fields](../../../../../scalar-field.md). The [scalar mass matrix](../../../../../scalar-mass-matrix.md) is diagonal in this basis:

$$
\boxed{m_{h_0}^2=2C^2(\alpha+N\beta)=-2m^2,\qquad m_{h_A}^2=2\alpha C^2\quad(A=1,\ldots,N^2-1),\qquad m_{P_A}^2=0\quad(A=0,\ldots,N^2-1).}
$$

Thus $H$ contains one massive singlet and a degenerate multiplet of $N^2-1$ massive fields in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) of the unbroken diagonal $SU(N)$. Both squared [masses](../../../../../mass.md) are strictly positive for the specified parameters. The $P$ fields are the $N^2$ [Goldstone bosons](../../../../../goldstone-boson.md) associated with the broken generators: $N^2-1$ traceless relative left-right rotations and one overall phase rotation.

[Goldstone's theorem](../../../../../goldstone-theorem.md) guarantees those massless directions. It does not alone forbid additional accidental massless modes; the positive [scalar mass matrix](../../../../../scalar-mass-matrix.md) computed here supplies the further conclusion that every $H$ component is massive. The fields describe a global symmetry, so these [Goldstone bosons](../../../../../goldstone-boson.md) are physical rather than being absorbed into massive [gauge bosons](../../../../../gauge-boson.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
