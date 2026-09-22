<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In this part the earlier variable $n$ specializes to six. A [group representation](../../../../group-representation.md) of $U(1)\times SU(6)$ factors through the [quotient group](../../../../quotient-group.md) $U(6)$ exactly when the central [subgroup](../../../../subgroup.md) $K$ in [solution](../b/solution.md) acts trivially. For an irreducible [SU(6)](../../../../su-6.md) [tensor](../../../../tensor.md) [representation](../../../../group-representation.md) represented by a [Young diagram](../../../../young-diagram.md) with $b$ boxes, the scalar [matrix](../../../../matrix.md) $\zeta^{-1}I_6$ acts as $\zeta^{-b}$, where $\zeta=e^{2\pi i/6}$.

The prescribed [representation](../../../../group-representation.md) $\widetilde R(z,U)=R(U)$ gives no compensating phase from the first factor. Its value on the generator of $K$ is therefore $R(\zeta^{-1}I_6)=\zeta^{-b}I$. The box counts in [solution](../c/solution.md) give

$$
\begin{array}{c|ccccc}
R&\mathbf6&\overline{\mathbf6}&\mathbf{21}&\mathbf{15}&\mathbf{35}\\\hline
b\pmod6&1&5&2&2&0\\
\widetilde R(\zeta,\zeta^{-1}I_6)&\zeta^{-1}I&\zeta I&\zeta^{-2}I&\zeta^{-2}I&I
\end{array}
$$

Consequently

$$
\boxed{\text{Among these prescribed lifts, only the adjoint }\mathbf{35}\text{ descends to }U(6).}
$$

Concretely, conjugation $T\mapsto WTW^{-1}$ defines it for every $W\in U(6)$, and the scalar phase cancels.

The qualification “prescribed lifts” matters. The defining [representation](../../../../group-representation.md) of $U(6)$ certainly exists, but its pullback is $(z,U)\mapsto zU$, not $(z,U)\mapsto U$. For instance $(\zeta,\zeta^{-1}I_6)$ and $(1,I_6)$ represent the same quotient element, while the latter prescription assigns them different [matrices](../../../../matrix.md) in the defining [representation](../../../../group-representation.md). More generally, for an integer $q$, a lift $z^qR(U)$ descends precisely when

$$
\boxed{q\equiv b\pmod6.}
$$

This [descent criterion for representations of U(n)](../../../../descent-criterion-for-representations-of-u-n.md) explains how all the listed [SU(6)](../../../../su-6.md) [representations](../../../../group-representation.md) can be extended after choosing a suitable first-factor [U(1) charge](../../../../u-1-charge.md), even though only one descends with that charge fixed to zero.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
