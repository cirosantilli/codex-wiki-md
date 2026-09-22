<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a positive-dimensional smooth connected manifold, three [equivalent formulations of orientability of a smooth manifold](../../../../../equivalent-formulations-of-orientability-of-a-smooth-manifold.md) are an [oriented atlas](../../../../../oriented-atlas.md), a continuously varying orientation of each [tangent space](../../../../../tangent-space.md), and a nowhere-vanishing smooth top-degree [differential form](../../../../../differential-form-split.md). An orientation of a [tangent space](../../../../../tangent-space.md) means a choice of one class of ordered bases, where two bases agree when their change-of-basis [determinant](../../../../../determinant.md) is positive. The second formulation chooses these classes locally continuously; it does not require a global frame.

An [oriented atlas](../../../../../oriented-atlas.md) has positive Jacobian [determinant](../../../../../determinant.md) on every overlap. Its coordinate bases then give a consistent orientation of all [tangent spaces](../../../../../tangent-space.md). Conversely, a continuous choice of tangent-space orientations makes the sign of a coordinate basis locally constant. Shrink to connected charts and reverse one coordinate when necessary; the resulting positively positively oriented coordinate charts have positive transition [determinants](../../../../../determinant.md). An orientation in atlas language is the maximal collection of charts compatible with that positive sign convention.

We use the [partition of unity](../../../../../partition-of-unity.md) theorem: every open cover of a Hausdorff second-countable [smooth manifold](../../../../../smooth-manifold.md) has a smooth locally finite subordinate partition. From the oriented atlas, choose such a [partition of unity](../../../../../partition-of-unity.md) $\rho_i$. Extend each $\rho_i\,dx_i^1\wedge\cdots\wedge dx_i^n$ by zero outside its chart and sum the locally finite family. At every point, the nonzero summands are positive multiples of one another and at least one coefficient is positive. Their sum is a smooth nowhere-zero form $\omega$. Conversely, a nowhere-zero form declares a basis positive exactly when $\omega(v_1,\ldots,v_n)>0$, giving a continuously varying orientation and hence an [oriented atlas](../../../../../oriented-atlas.md). Two top forms define the same orientation precisely when $\omega'=h\omega$ for a smooth positive function $h$. Since a nonvanishing coefficient cannot change sign on a connected manifold, these definitions give exactly two opposite orientations.

For the unit sphere in $\mathbb R^{n+1}$, define

$$
\boxed{\omega_x(v_1,\ldots,v_n)=\det(x,v_1,\ldots,v_n)}.
$$

The radial vector $x$ is a unit normal, so appending any tangent basis gives an ambient basis and the [determinant](../../../../../determinant.md) never vanishes. The form is smooth and provides the outward-normal-first orientation. Therefore $\boxed{S^n\text{ is orientable for every }n}$. For $n=0$, this is the nonzero zero-form taking opposite signs on the two sphere points; zero-dimensional manifolds admit orientations by assigning generator signs at their points.

For $n\ge1$, the quotient map $\pi:S^n\to\mathbb{RP}^n$ is a twofold smooth covering with [deck transformation](../../../../../deck-transformation.md) $A(x)=-x$. Its action on the sphere form is

$$
(A^*\omega)_x(v_1,\ldots,v_n)=\det(-x,-v_1,\ldots,-v_n)
=(-1)^{n+1}\omega_x(v_1,\ldots,v_n).
$$

If $n$ is odd, the form is invariant and descends using the local covering inverses to a nowhere-vanishing form on the quotient. If $n$ is even, suppose the quotient had a nonvanishing top form $\eta$. Its pullback would be $h\omega$ for a smooth nonzero function $h$ on the connected sphere and would be invariant under $A$. Invariance would require $h(-x)=-h(x)$, impossible because $h$ has constant sign. This proves the [orientability of real projective space](../../../../../orientability-of-real-projective-space.md) criterion

$$
\boxed{\mathbb{RP}^n\text{ is orientable exactly when }n\text{ is odd, for }n\ge1}.
$$

The separate endpoint $\mathbb{RP}^0$ is one point and is orientable, so the full nonnegative-dimensional answer is $n=0$ or $n$ odd.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
