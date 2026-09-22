<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [fundamental-doublet breaking of SU(2)](../../../../../fundamental-doublet-breaking-of-su-2.md), assume $\lambda>0$ and $v>0$. The minima of the [scalar potential](../../../../../scalar-potential.md) satisfy $\phi^\dagger\phi=v^2/2$, giving a three-sphere [vacuum manifold](../../../../../vacuum-manifold.md). A chosen [vacuum expectation value](../../../../../vacuum-expectation-value.md) is $\phi_0=(0,v)^T/\sqrt2$. No nonzero generator $a_a\tau^a$ annihilates $\phi_0$: its squared norm is $v^2(a_1^2+a_2^2+a_3^2)/8$. At the group level, an $SU(2)$ matrix fixing the nonzero vector $\phi_0$ must be the identity. Thus all three generators of the [SU(2) gauge theory](../../../../../su-2-gauge-theory.md) are broken in the usual perturbative [Higgs mechanism](../../../../../higgs-mechanism.md) description.

Make the radial and angular fields explicit:

$$
\phi(x)=\exp\left(\frac{i\sigma^a\pi^a(x)}v\right)\frac1{\sqrt2}\begin{pmatrix}0\\v+h(x)\end{pmatrix}.
$$

A local [gauge transformation](../../../../../gauge-transformation.md) removes the three angular fields $\pi^a$. In [unitary gauge](../../../../../unitary-gauge.md), the [Pauli matrices](../../../../../pauli-matrices.md) identity $\{\tau^a,\tau^b\}=\delta^{ab}\mathbf1/2$ gives

$$
(D_\mu\phi)^\dagger D^\mu\phi=\frac12(\partial_\mu h)(\partial^\mu h)+\frac{g^2}{8}(v+h)^2A_\mu^aA^{a\mu}.
$$

The mixed derivative term cancels between a term and its complex conjugate. The [scalar potential](../../../../../scalar-potential.md) becomes

$$
V=\lambda\left(vh+\frac{h^2}{2}\right)^2=\lambda v^2h^2+\lambda vh^3+\frac\lambda4h^4.
$$

Consequently the complete physical [Lagrangian density](../../../../../lagrangian-density.md) is

$$
\begin{aligned}
\mathcal L={}&-\frac14F_{\mu\nu}^aF^{a\mu\nu}+\frac12(\partial h)^2
+\frac12m_A^2A_\mu^aA^{a\mu}-\frac12m_h^2h^2\\
&+\frac{g^2v}{4}hA_\mu^aA^{a\mu}+\frac{g^2}{8}h^2A_\mu^aA^{a\mu}-\lambda vh^3-\frac\lambda4h^4,\\
F_{\mu\nu}^a={}&\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+g\epsilon^{abc}A_\mu^bA_\nu^c.
\end{aligned}
$$

Reading the quadratic terms with their canonical factors $1/2$ gives

$$
\boxed{m_{A^1}=m_{A^2}=m_{A^3}=\frac{gv}{2},\qquad m_h=\sqrt{2\lambda}\,v.}
$$

All physical scalar-vector and scalar self-interactions are displayed in the second line of $\mathcal L$. In particular the new cubic couplings proportional to $v$ are $hA^aA^a$ and $h^3$. Their [Feynman vertices](../../../../../interaction-vertex.md), together with the quartic ones, are

$$
\boxed{hA_\mu^aA_\nu^b:\ i\frac{g^2v}{2}\delta^{ab}g_{\mu\nu},\quad hhA_\mu^aA_\nu^b:\ i\frac{g^2}{2}\delta^{ab}g_{\mu\nu},\quad hhh:\ -6i\lambda v,\quad hhhh:\ -6i\lambda.}
$$

The three-vector and four-vector interactions are already contained in the non-Abelian [gauge field strength](../../../../../gauge-field-strength.md) term. There are no further physical fields or interactions in this specified model. Before fixing [unitary gauge](../../../../../unitary-gauge.md), the quadratic angular term is $\tfrac12(\partial_\mu\pi^a-m_AA_\mu^a)^2$. It exhibits three zero-curvature angular directions of the [scalar potential](../../../../../scalar-potential.md), but also their mixing with the [gauge fields](../../../../../gauge-field.md). They supply the third [polarization](../../../../../polarization-waves.md) of each massive [gauge boson](../../../../../gauge-boson.md), rather than massless physical [particles](../../../../../particle-physics.md).

The degrees of freedom count is $3\cdot2+4=10$ before breaking and $3\cdot3+1=10$ afterwards. If instead the symmetry were global, as in the decoupled $g=0$ scalar theory, the three angular fields would be physical massless [Goldstone bosons](../../../../../goldstone-boson.md). This is consistent with [Goldstone's theorem](../../../../../goldstone-theorem.md). The language of a broken local symmetry refers to this gauge-fixed expansion; a gauge-dependent [vacuum expectation value](../../../../../vacuum-expectation-value.md) is not itself a gauge-invariant observable.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
