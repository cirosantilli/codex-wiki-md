<h1 id="e8/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The premise contains a wording error: $\lambda$ must be a nonzero **[eigenvalue](../../../../../../eigenvalue.md)**, rather than a nonzero [eigenvector](../../../../../../eigenvector.md). Let $v\ne0$ satisfy

$$
X^TXv=\lambda v,\qquad \lambda\ne0.
$$

Then $Xv\ne0$, since otherwise $X^TXv=0$ would force $\lambda v=0$. Multiplying by $X$ gives

$$
XX^T(Xv)=X(X^TXv)=\lambda(Xv).
$$

Thus **$\boxed{\lambda\text{ is an eigenvalue of }XX^T}$**, with [eigenvector](../../../../../../eigenvector.md) $Xv$. Conversely, applying $X^T$ maps an [eigenvector](../../../../../../eigenvector.md) of $XX^T$ with nonzero [eigenvalue](../../../../../../eigenvalue.md) to one of $X^TX$.

These maps are inverses up to the factor $\lambda$ on the corresponding [eigenspaces](../../../../../../eigenspace.md), so the nonzero [eigenvalues](../../../../../../eigenvalue.md) have equal multiplicities. Their zero [eigenvalues](../../../../../../eigenvalue.md) need not have the same multiplicity because the two [matrices](../../../../../../matrix.md) can have different sizes. For a unit [eigenvector](../../../../../../eigenvector.md) $v$ and real $X$, the normalized partner is $u=Xv/\sqrt\lambda$, since $\|Xv\|^2=v^TX^TXv=\lambda>0$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [E](../../e.md)
3. [E8](../../../e8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../../split.md)
7. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
