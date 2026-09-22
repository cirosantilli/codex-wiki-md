<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the local positive $\widetilde z$ axis along the [classical spin](../../../../classical-spin.md). For nonzero [field](../../../../magnetic-field-split.md), a [proper rotation](../../../../rotation-mathematics.md) is

$$
\boxed{S_j^x=s\widetilde S_j^z,\qquad S_j^y=\widetilde S_j^y,\qquad S_j^z=-s\widetilde S_j^x.}
$$

It preserves the [Spin commutation relations](../../../../spin-commutation-relations.md) and turns the [field](../../../../magnetic-field-split.md) term into $-H_fS\sum_j\widetilde S_j^z$. At zero [field](../../../../magnetic-field-split.md) choose the classical direction $+x$, so $s=1$. Expanding about the original $z$ axis without this [rotation](../../../../rotation-mathematics.md) would put the reference state away from the classical minimum and would not give a controlled small-deviation expansion.

To the required order,

$$
\widetilde S_j^z=S-n_j,\qquad
\widetilde S_j^x=\sqrt{\frac S2}(a_j+a_j^\dagger)+O(S^{-1/2}),\qquad
\widetilde S_j^y=-i\sqrt{\frac S2}(a_j-a_j^\dagger)+O(S^{-1/2}).
$$

The longitudinal exchange gives $-JS^2+JS(n_j+n_{j+1})+O(S^0)$ on each bond. The transverse exchange gives

$$
-J\widetilde S_j^y\widetilde S_{j+1}^y
=\frac{JS}{2}\left[a_ja_{j+1}+a_j^\dagger a_{j+1}^\dagger-a_j^\dagger a_{j+1}-a_{j+1}^\dagger a_j\right]+O(S^0).
$$

Finally the [field](../../../../magnetic-field-split.md) contributes its classical constant and $H_fSn_j$. Each site belongs to two bonds, so after removing the order-$S^2$ constant,

$$
\boxed{A=-\frac{JS}{2},\qquad B=\frac{JS}{2},\qquad C=S(2J+H_f).}
$$

These are the order-$S$ terms; the discarded products of [number operators](../../../../number-operator.md) and the next square-root terms are order $S^0$ for [occupations](../../../../bosonic-occupation-number.md) held fixed as $S\to\infty$. A different transverse-axis phase can reverse the sign of $B$ without changing the [spectrum](../../../../energy-eigenvalue-split.md), but the sign above follows from the stated [rotation](../../../../rotation-mathematics.md) and oscillator convention.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
