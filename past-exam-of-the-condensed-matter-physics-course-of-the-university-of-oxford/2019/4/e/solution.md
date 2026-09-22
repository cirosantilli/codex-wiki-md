<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $s=\langle S_i^z\rangle$ be uniform, with dimensionless spin operators $S=1/2$. The factor $1/2$ in the source Hamiltonian removes double counting of pairs. Decoupling $\mathbf S_i\cdot\mathbf S_j$ about a uniform polarization gives the one-site [mean-field theory](../../../../mean-field-theory.md) Hamiltonian

$$
H_i^{\mathrm{MF}}=-sJ_0S_i^z+\mathrm{constant},\qquad J_0=\sum_jJ_{ij}.
$$

A body-centred-cubic site has eight nearest neighbors and six next-nearest neighbors, so

$$
\frac{J_0}{k_B}=8(1\,\mathrm{mK})+6(-0.5\,\mathrm{mK})=5\,\mathrm{mK}.
$$

For a spin one half in this effective field, the [mean-field self-consistency equation](../../../../self-consistency-equation.md) is

$$
s=\frac12\tanh\left(\frac{J_0s}{2k_BT}\right).
$$

Linearizing at the continuous onset gives $s=J_0s/(4k_BT)+O(s^3)$, hence

$$
\boxed{T_C^{\mathrm{MF}}=\frac{J_0}{4k_B}=1.25\,\mathrm{mK}.}
$$

Equivalently, the general spin-$S$ result is $k_BT_C^{\mathrm{MF}}=S(S+1)J_0/3$. The antiferromagnetic next-nearest-neighbor exchange reduces the uniform ordering scale rather than contributing its absolute magnitude. The negative nuclear [g-factor](../../../../g-factor-physics.md) does not change this exchange instability; aligning the spins also aligns their moments with one another.

For these particular competing couplings, the uniform mode is indeed the largest exchange eigenvalue. Writing $x=\cos(q_xa/2)$, $y=\cos(q_ya/2)$ and $z=\cos(q_za/2)$ gives

$$
\frac{J(\mathbf q)}{k_B\,\mathrm{mK}}=8xyz-2(x^2+y^2+z^2)+3\le5,
$$

with equality at $\mathbf q=0$ modulo [reciprocal lattice vectors](../../../../reciprocal-lattice-vector.md). To see the bound, replace a negative $xyz$ by its absolute value for an upper bound, let $t=(|xyz|)^{1/3}$, and use $x^2+y^2+z^2\ge3t^2$. The expression is at most $8t^3-6t^2+3$, whose maximum on $0\le t\le1$ is five. Thus another modulation does not preempt the stated ferromagnetic onset at this level of [mean-field theory](../../../../mean-field-theory.md). Fluctuations can change the actual transition temperature.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
