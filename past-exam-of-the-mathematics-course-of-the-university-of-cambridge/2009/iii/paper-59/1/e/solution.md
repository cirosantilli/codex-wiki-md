<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [chiral spinor curvature operator](../../../../../../chiral-spinor-curvature-operator.md) acts algebraically on a two-dimensional spinor space. We may therefore lower its matrix index using the [symplectic form](../../../../../../symplectic-form.md) and write $\Delta_{AB}\alpha_C=X_{ABDC}\alpha^D$. Symmetry of $\Delta_{AB}$ gives symmetry in the first pair of $X$. Preservation of $\epsilon_{CD}$ says that its action is symplectic; lowering the endomorphism index of a symplectic infinitesimal transformation makes a symmetric two-index tensor. Thus $X_{ABCD}=X_{(AB)(CD)}$.

The additional [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) symmetry $R_{abcd}=R_{cdab}$ implies $X_{ABCD}=X_{CDAB}$: project both antisymmetric spacetime index pairs onto the unprimed chiral summand. Equivalently this is the symmetry of the unprimed diagonal block of the curvature operator on [differential two-forms](../../../../../../2-form.md). The [contracted chiral curvature identity](../../../../../../contracted-chiral-curvature-identity.md) is another way of expressing the same three constraints on the initially nine-component pair-symmetric spinor.

Consequently $X$ is a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) on the three-dimensional space $\operatorname{Sym}^2 S$, with six independent components. Its total symmetrization $\Psi_{ABCD}=X_{(ABCD)}$ has five components. The one-dimensional remainder is spanned by

$$
K_{ABCD}=-\epsilon_{D(A}\epsilon_{B)C}=-\frac12(\epsilon_{DA}\epsilon_{BC}+\epsilon_{DB}\epsilon_{AC}).
$$

It is symmetric within and between pairs, and $K_{(ABCD)}=0$. The latter follows from the two-dimensional alternating-form identity, or directly by evaluating its components with $\epsilon_{01}=1$. Hence the [chiral Riemann curvature spinor decomposition](../../../../../../chiral-riemann-curvature-spinor-decomposition.md) is

$$
\boxed{X_{ABCD}=\Psi_{ABCD}-\Lambda\epsilon_{D(A}\epsilon_{B)C},\qquad\Psi_{ABCD}=\Psi_{(ABCD)}.}
$$

A contraction of a totally symmetric spinor with an [symplectic form](../../../../../../symplectic-form.md) vanishes. Meanwhile the explicit two-term expression for $K$ gives $K_{ABCD}\epsilon^{AC}\epsilon^{BD}=3$. Therefore the scalar in the printed normalization is

$$
\boxed{\Lambda=\frac13X_{ABCD}\epsilon^{AC}\epsilon^{BD}.}
$$

In particular, $\Psi=X-\Lambda K$ has zero such trace and is the [Weyl curvature spinor](../../../../../../weyl-curvature-spinor.md). The coefficient is fixed by the factor implicit in the printed symmetrization; substituting a differently normalized scalar-curvature term would change the relation between its scalar parameter and this contraction.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
