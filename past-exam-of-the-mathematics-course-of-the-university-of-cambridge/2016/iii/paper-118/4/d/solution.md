<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal P=\mathcal M_X/\mathcal O_X$, the [sheaf of meromorphic principal parts](../../../../../../sheaf-of-meromorphic-principal-parts.md). Exactness of taking [stalks](../../../../../../stalk-of-a-sheaf.md) gives

$$
\mathcal P_x=\mathcal M_{X,x}/\mathcal O_{X,x}.
$$

Choose a [holomorphic coordinate](../../../../../../holomorphic-coordinate.md) $t$ vanishing at $x$. Every meromorphic germ has a finite negative tail in its [Laurent series](../../../../../../laurent-series.md); the holomorphic tail vanishes in the quotient. Hence

$$
\boxed{\mathcal P_x\cong\bigoplus_{m\geq1}\mathbb C\,t^{-m}.}
$$

This coordinate description is a vector-space identification; the intrinsic space is the quotient of germs, so a coordinate change need not preserve the displayed basis.

For each point inclusion $i_x:\{x\}\to X$, a principal part defines a local meromorphic germ near $x$, whose quotient class is zero off $x$. Gluing with zero on the complement gives a map from its [skyscraper sheaf](../../../../../../skyscraper-sheaf.md) to $\mathcal P$. These maps induce an isomorphism on every stalk and therefore an isomorphism of sheaves:

$$
\boxed{\mathcal P\cong\bigoplus_{x\in X}(i_x)_*\mathcal P_x.}
$$

The [direct sum of sheaves](../../../../../../direct-sum-of-sheaves.md) means the sheafification of the sectionwise direct-sum presheaf. Its sections can have infinitely many nonzero components globally, but their point supports form a [locally finite family of subsets](../../../../../../locally-finite-family-of-subsets.md). This matches the fact that poles of a [meromorphic function](../../../../../../meromorphic-function.md) are locally finite. On a compact [Riemann surface](../../../../../../riemann-surfaces.md) only finitely many points can occur; on a noncompact one a discrete infinite family is allowed.

For a global principal-part family $P$, choose local meromorphic lifts $m_i$ on a sufficiently small [open cover](../../../../../../open-cover.md). The differences $m_j-m_i$ are [holomorphic functions](../../../../../../holomorphic-function.md) and form a [Čech cocycle](../../../../../../cech-cocycle-condition.md). The [connecting homomorphism](../../../../../../connecting-homomorphism.md) sends $P$ to the resulting class in $H^1(X,\mathcal O_X)$. If this class vanishes, after refining the cover write $m_j-m_i=h_j-h_i$; then the functions $m_i-h_i$ glue to a global [meromorphic function](../../../../../../meromorphic-function.md). Conversely any global lift makes the class zero. Equivalently, exactness of the given [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) says

$$
\boxed{\delta(P)=0\iff\text{there is a global meromorphic function with exactly the prescribed principal parts}.}
$$

**The connecting class is the obstruction to the Mittag-Leffler problem on a Riemann surface.** It rules on the specified poles and their finite negative Laurent tails, with no additional poles allowed. When a solution exists, any two solutions differ by a global [holomorphic function](../../../../../../holomorphic-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
