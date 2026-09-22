<h1 id="p/p4/solution">Solution</h1>

↑ **Parent:** [P4](../p4.md)

For a nonzero real vector $w$, a [Householder reflection](../../../../householder-transformation.md) is

$$
H(w)=I-\frac{2ww^T}{w^Tw}.
$$

Writing $P=ww^T/(w^Tw)$ gives $P^T=P$ and $P^2=P$, so $H^TH=(I-2P)^2=I$. Thus a [Householder matrix](../../../../householder-transformation.md) is an [orthogonal matrix](../../../../orthogonal-matrix.md), and it reflects across the [hyperplane](../../../../hyperplane.md) perpendicular to $w$.

For $u\ne0$, choose $\alpha=-\operatorname{sgn}(u_1)\|u\|$, taking the sign to be $+1$ when $u_1=0$, and put $w=u-\alpha e_1$. This $w$ is nonzero. Since $\alpha^2=\|u\|^2$, direct expansion gives $w^Tw=2(\|u\|^2-\alpha u_1)$ and $w^Tu=\|u\|^2-\alpha u_1$, so

$$
\boxed{H(w)u=\alpha e_1}.
$$

Apply this construction successively to the trailing part of each column of $A$, extending each [reflection](../../../../reflection-mathematics.md) by an identity on earlier coordinates. Previously created zeros are preserved. If a trailing column vector is zero, use the identity there. The resulting product $Q^T$ is [orthogonal](../../../../orthogonal-vectors.md) and $Q^TA=R$ is [upper triangular](../../../../upper-triangular-matrix.md), yielding the [QR factorization](../../../../qr-decomposition.md) $A=QR$ even when $A$ is singular.

To solve $Ax=b$, multiply by $Q^T$ and use [back substitution](../../../../back-substitution.md) on $Rx=Q^Tb$ when $R$ is nonsingular. If $A$ is singular, $\det R=\det(Q^T)\det A=0$; an [upper triangular](../../../../upper-triangular-matrix.md) [determinant](../../../../determinant.md) is its diagonal product, so at least one diagonal entry is zero. In that case consistency and free variables require separate treatment.

The unshifted [QR algorithm](../../../../qr-algorithm.md) starts from $A_0=A$, factors $A_k=Q_kR_k$, and forms

$$
\boxed{A_{k+1}=R_kQ_k=Q_k^TA_kQ_k}.
$$

Every iterate is related by an [orthogonal](../../../../orthogonal-vectors.md) [similarity transformation](../../../../similarity-transformation.md) to the previous one and hence to $A$, with the same [eigenvalues](../../../../eigenvalue.md). Symmetry is preserved. For symmetric matrices with appropriate spectral separation, the iterates approach diagonal form: the off-diagonal entries decrease and the diagonal exposes the eigenvalues. Practical shifted QR accelerates convergence and uses deflation when off-diagonal couplings become negligible. With a shift $\mu_k$, factor $A_k-\mu_kI=Q_kR_k$ and set $A_{k+1}=R_kQ_k+\mu_kI$; the same similarity identity still holds.

Universal diagonal convergence of unshifted QR would be too strong. For example $A=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ admits the standard factorization $Q=A$, $R=I$, so the iteration remains at $A$ rather than becoming diagonal, although its eigenvalues are $\pm1$. Such equal-modulus cases require a convergence qualification or treatment of a retained block. Similarity is unconditional; convergence to a useful limiting form is an additional algorithmic property.

## ↑ Ancestors (12)

1. [P4](../p4.md)
2. [P](../../p.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
