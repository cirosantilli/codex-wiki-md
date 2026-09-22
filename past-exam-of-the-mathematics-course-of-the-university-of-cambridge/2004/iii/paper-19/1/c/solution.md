<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand a [Jacobi field](../../../../../../jacobi-field.md) in the parallel orthonormal [eigenbasis](../../../../../../eigenbasis.md): $J(t)=\sum_i j_i(t)e_i(t)$. Part (b) reduces its equation to the scalar equations $j_i''+\lambda_i j_i=0$. Define

$$
S_\lambda(t)=\begin{cases}
\sin(\sqrt\lambda\,t)/\sqrt\lambda,&\lambda>0,\\
t,&\lambda=0,\\
\sinh(\sqrt{-\lambda}\,t)/\sqrt{-\lambda},&\lambda<0,
\end{cases}
\qquad C_\lambda(t)=S_\lambda'(t).
$$

For arbitrary initial values $J(0)=\sum_i a_ie_i$ and $D_tJ(0)=\sum_i b_ie_i$, the complete solution is

$$
J(t)=\sum_i\bigl(a_iC_{\lambda_i}(t)+b_iS_{\lambda_i}(t)\bigr)e_i(t).
$$

A point at parameter $T>0$ is a [conjugate point](../../../../../../conjugate-point.md) of $p$ precisely when a nonzero [Jacobi field](../../../../../../jacobi-field.md) vanishes at both $0$ and $T$. The first condition makes every $a_i=0$. The second requires $b_iS_{\lambda_i}(T)=0$ for every $i$, with at least one nonzero $b_i$. For $T>0$, the factors for zero and negative [eigenvalues](../../../../../../eigenvalue.md) never vanish; positive [eigenvalues](../../../../../../eigenvalue.md) give exactly the sine zeros. Therefore

$$
\boxed{T=\frac{k\pi}{\sqrt{\lambda_i}},\qquad k\in\mathbb N_{>0},\quad\lambda_i>0.}
$$

The corresponding points are $\gamma(T)$. If several positive eigenspaces have a zero at the same parameter, the conjugate multiplicity is the sum of their dimensions. This also shows that a [locally symmetric Riemannian manifold](../../../../../../locally-symmetric-riemannian-manifold.md) has no [conjugate points](../../../../../../conjugate-points.md) along a given [geodesic](../../../../../../geodesic.md) when that [geodesic](../../../../../../geodesic.md)'s [Jacobi curvature operator](../../../../../../jacobi-curvature-operator.md) has no positive [eigenvalues](../../../../../../eigenvalue.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
