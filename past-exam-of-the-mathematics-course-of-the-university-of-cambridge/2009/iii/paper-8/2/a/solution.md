<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) says that a compact self-adjoint $A$ has an orthogonal decomposition

$$
H=\ker A\oplus\mathop{\widehat\bigoplus}_{\lambda\ne0}\ker(A-\lambda I),
$$

with real nonzero [eigenvalues](../../../../../../eigenvalue.md) of finite multiplicity. Only finitely many [eigenvalues](../../../../../../eigenvalue.md), counting multiplicity, have absolute value at least any given $\varepsilon>0$. Thus the nonzero [eigenvalues](../../../../../../eigenvalue.md) form a finite list or a sequence tending to zero, and $A=\sum_{\lambda\ne0}\lambda P_\lambda$ in operator norm. The kernel may have arbitrary Hilbert dimension.

For existence of an extremal [eigenvector](../../../../../../eigenvector.md), self-adjointness gives $\|A\|=\sup_{\|x\|=1}|\langle Ax,x\rangle|$. One elementary proof of the nontrivial inequality uses polarization: if the quadratic form is bounded in absolute value by $m\|x\|^2$, its polarized real part is bounded by $m$ on two unit vectors; adjusting a phase bounds $|\langle Ax,y\rangle|$ by $m$. Choose unit $x_j$ with quadratic values tending to $\lambda=\|A\|$ or $-\|A\|$. Then

$$
\|(A-\lambda)x_j\|^2\leq2\|A\|^2-2\lambda\langle Ax_j,x_j\rangle\longrightarrow0.
$$

If $A\ne0$, compactness supplies a convergent subsequence of $Ax_j$, and the last estimate supplies a convergent unit subsequence of $x_j$, with [eigenvalue](../../../../../../eigenvalue.md) $\lambda$.

[Eigenvectors](../../../../../../eigenvector.md) for distinct [eigenvalues](../../../../../../eigenvalue.md) are orthogonal, since $A=A^*$. An infinite orthonormal sequence in one nonzero eigenspace would violate compactness. More generally an infinite orthonormal family with [eigenvalues](../../../../../../eigenvalue.md) bounded away from zero has images separated in norm, again impossible. Take all nonzero eigenspaces and let $M$ be their closed span. Its complement reduces $A$; if the restriction there were nonzero, the extremal-eigenvector argument would produce another nonzero [eigenvector](../../../../../../eigenvector.md), a contradiction. Thus $M^\perp=\ker A$. The finite truncations of the [eigenvalue](../../../../../../eigenvalue.md) sum have remainder norm tending to zero, proving the asserted norm expansion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
