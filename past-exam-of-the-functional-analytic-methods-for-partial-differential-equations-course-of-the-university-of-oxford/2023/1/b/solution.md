<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the unbounded domain $\mathbb R^3$, translations already prevent [compactness](../../../../compact-space.md) in every indicated [Hölder space](../../../../holder-space.md). Choose a [bump function](../../../../bump-function.md) $\eta\in C_c^\infty(B_1)$ with $\eta(0)=1$, put $e_1=(1,0,0)$, and define

$$
\boxed{u_m(x)=\eta(x-3m e_1),\qquad m=1,2,\ldots.}
$$

A [change of variables](../../../../change-of-variables-formula.md) in the [Lebesgue integrals](../../../../lebesgue-integral.md) defining the [Sobolev norm](../../../../sobolev-norm.md) gives $\|u_m\|_{W^{1,6}(\mathbb R^3)}=\|\eta\|_{W^{1,6}(\mathbb R^3)}$, so the sequence is bounded. Each $u_m$ is a [smooth function](../../../../smooth-function.md) of [compact support](../../../../compact-support.md) and belongs to every [Hölder space](../../../../holder-space.md) $C^{0,\gamma}(\mathbb R^3)$, $0<\gamma\leq1$: its bounded [gradient](../../../../gradient.md) gives the [Lipschitz](../../../../lipschitz-continuity.md) estimate for distances at most one, and its bounded values control larger distances.

For $m\ne\ell$, the [supports](../../../../support.md) are disjoint, and at $x=3m e_1$ we have $u_m(x)=1$ and $u_\ell(x)=0$. Therefore

$$
\|u_m-u_\ell\|_{C^{0,\gamma}}\geq\|u_m-u_\ell\|_\infty\geq1
\qquad(0<\gamma\leq1).
$$

No [subsequence](../../../../subsequence.md) can be a [Cauchy sequence](../../../../cauchy-sequence.md) in any of these [Hölder norms](../../../../holder-norm.md), hence none converges. This uses the translation mechanism for [noncompactness of a Sobolev embedding by translation](../../../../noncompactness-of-a-sobolev-embedding-by-translation.md); concentration at the critical [Hölder exponent](../../../../holder-exponent.md) alone would not rule out convergence at every smaller [Hölder exponent](../../../../holder-exponent.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
