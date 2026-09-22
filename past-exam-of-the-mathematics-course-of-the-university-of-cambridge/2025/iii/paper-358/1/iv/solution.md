<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $Q_n=P_n=P_n^*$ for the orthogonal projections and regard the compression $A_n=Q_nAQ_n$ as acting on $\operatorname{ran}Q_n$. The compactness argument from part iii applies to any strongly convergent sequence of orthogonal projections, so

$$
\boxed{\|A-A_n\|\to0}.
$$

We first rule out spectral pollution. Suppose $\lambda_n\in\operatorname{Sp}(A_n)$ and, after taking a subsequence, $\lambda_n\to\lambda\ne0$. Choose unit eigenvectors $x_n\in\operatorname{ran}Q_n$:

$$
A_nx_n=\lambda_nx_n.
$$

Compactness gives a convergent subsequence of $Ax_n$. Because

$$
\|(A-A_n)x_n\|\to0,
$$

the relation $x_n=\lambda_n^{-1}A_nx_n$ then makes $x_n$ converge to a nonzero vector $x$, and passage to the limit gives $Ax=\lambda x$. Thus every nonzero limit of finite-section spectral points belongs to $\operatorname{Sp}(A)$. The only remaining possible limit is zero, which belongs to the spectrum of a compact operator on an infinite-dimensional space.

Conversely, the [Riesz–Schauder theorem](../../../../../../riesz-schauder-theorem.md) says that every nonzero $\lambda\in\operatorname{Sp}(A)$ is an isolated eigenvalue of finite algebraic multiplicity. Put a small contour around $\lambda$ containing no other point of $\operatorname{Sp}(A)$. Norm convergence of $A_n$ gives uniform resolvent convergence on the contour, so the associated Riesz projections converge in norm and eventually have the same positive rank. Hence $\operatorname{Sp}(A_n)$ meets every neighborhood of $\lambda$.

Finally, zero is also approximated. Otherwise some subsequence would have all its eigenvalues bounded away from zero. Outside any small disk, $\operatorname{Sp}(A)$ has only finitely many eigenvalues, and the preceding Riesz-projection argument fixes the total algebraic multiplicity of nearby finite-section eigenvalues. This cannot account for

$$
\dim\operatorname{ran}Q_n\longrightarrow\infty.
$$

Thus finite-section eigenvalues also approach zero. Both directed spectral distances vanish, proving

$$
\boxed{
d_H\bigl(\operatorname{Sp}(P_nAP_n^*),
\operatorname{Sp}(A)\bigr)\longrightarrow0}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
