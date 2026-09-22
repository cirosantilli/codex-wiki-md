<h1 id="8b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a real [antisymmetric matrix](../../../../../../skew-symmetric-matrix.md), $A^T=-A$, so $(A^2)^T=A^2$. The previous result makes every [eigenvalue](../../../../../../eigenvalue.md) $\eta$ of $A^2$ real, with a real nonzero [eigenvector](../../../../../../eigenvector.md) $v$. Moreover,

$$
\eta|v|^2=v^TA^2v=-(Av)^TAv=-|Av|^2\le0.
$$

Thus **every [eigenvalue](../../../../../../eigenvalue.md) of $A^2$ is real and nonpositive**.

Take real unit [eigenvectors](../../../../../../eigenvector.md) $u,w$ of $A^2$ for the respective distinct nonzero [eigenvalues](../../../../../../eigenvalue.md) $-\lambda^2,-\mu^2$, where the real parameters $\lambda,\mu$ are nonzero. Define

$$
u'=\frac{Au}{\lambda},\qquad w'=\frac{Aw}{\mu}.
$$

The displayed quadratic identity gives $|u'|=|w'|=1$. Also $u\cdot Au=0$ and $w\cdot Aw=0$, because a real [antisymmetric matrix](../../../../../../skew-symmetric-matrix.md) has zero [quadratic form](../../../../../../quadratic-form.md). Thus $u\perp u'$ and $w\perp w'$. Since $A$ commutes with $A^2$, $u'$ lies in the same [eigenspace](../../../../../../eigenspace.md) of $A^2$ as $u$, and $w'$ in the same one as $w$. Distinct [eigenspaces](../../../../../../eigenspace.md) of the real [symmetric matrix](../../../../../../symmetric-matrix.md) $A^2$ are [orthogonal](../../../../../../orthogonal-vectors.md), so all four [vectors](../../../../../../vector.md) are [orthonormal](../../../../../../orthonormal-set.md). Finally,

$$
\boxed{Au=\lambda u',\quad Au'=-\lambda u,\qquad
Aw=\mu w',\quad Aw'=-\mu w.}
$$

Thus on each of the two perpendicular planes, $A$ acts as a scaled quarter-turn. This constructs the required [vectors](../../../../../../vector.md), rather than merely counting dimensions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
