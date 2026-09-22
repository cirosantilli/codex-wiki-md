<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Lie group](../../../../../lie-group.md) is a finite-dimensional [smooth manifold](../../../../../smooth-manifold.md) with a group structure for which multiplication and inversion are smooth. The group defined here is the [compact symplectic group](../../../../../compact-symplectic-group.md) $Sp(n)=U(2n)\cap Sp(2n,\mathbb C)$, rather than the full complex symplectic group. Also, the displayed matrix expression requires $B$ to be $2n\times2n$; the printed $n\times n$ size is incompatible with $J$.

Since $J^2=-I$, we have $J^{-1}=-J$. The [matrix exponential](../../../../../matrix-exponential.md) commutes with conjugation, as follows term by term from its absolutely convergent [power series](../../../../../power-series.md). Consequently

$$
e^{-JBJ}=e^{JBJ^{-1}}=Je^BJ^{-1}=-Je^BJ.
$$

To construct [logarithm charts for the compact symplectic group](../../../../../logarithm-charts-for-the-compact-symplectic-group.md), consider the real [vector space](../../../../../vector-space-split.md)

$$
\mathfrak k=\{X:X^*=-X,\quad XJ+JX^t=0\}.
$$

Differentiating the defining identities at $I$ gives precisely these conditions. Conversely if $X\in\mathfrak k$, $e^X$ is unitary and

$$
\frac d{dt}(e^{tX}Je^{tX^t})=e^{tX}(XJ+JX^t)e^{tX^t}=0,
$$

so $e^X\in Sp(n)$. These are the infinitesimal conditions of the [compact symplectic Lie algebra](../../../../../compact-symplectic-lie-algebra.md).

Near $I$, the convergent [matrix logarithm](../../../../../matrix-logarithm.md) series $\log(I+C)=\sum_{m\ge1}(-1)^{m+1}C^m/m$ is smooth and inverse to the [matrix exponential](../../../../../matrix-exponential.md) near zero. These local inverses respect transpose, conjugate transpose, and conjugation; also $\log(A^{-1})=-\log A$ when both matrices are sufficiently close to $I$. Shrink their neighborhoods accordingly. If $A\in Sp(n)$ there, unitarity gives

$$
(\log A)^*=\log(A^*)=\log(A^{-1})=-\log A.
$$

The symplectic identity is equivalent to $A^t=J^{-1}A^{-1}J$, so, putting $X=\log A$, it gives $X^t=-J^{-1}XJ=JXJ$, equivalently $XJ+JX^t=0$. Thus this local logarithm restricts to a bijection between a neighborhood of $I$ in $Sp(n)$ and an open neighborhood of zero in $\mathfrak k$. Its inverse is the restricted [matrix exponential](../../../../../matrix-exponential.md). These restrictions are [manifold charts](../../../../../manifold-chart.md); left multiplication translates them to every $A_0\in Sp(n)$ via $A\mapsto\log(A_0^{-1}A)$. The chart overlaps are smooth compositions of multiplication, exponential and logarithm. The subspace topology is Hausdorff and second countable, inherited from the finite-dimensional matrix space, so these charts give a [smooth manifold](../../../../../smooth-manifold.md).

Closure under products and inverses follows from $AJ A^t=J$ and unitarity. Matrix multiplication is polynomial in real and imaginary entries, and inversion on the unitary group is $A\mapsto A^*$, a real linear operation. Their restrictions are smooth in the charts just constructed. Hence $Sp(n)$ is a [Lie group](../../../../../lie-group.md) without needing a closed-subgroup theorem.

Write $X$ in $n\times n$ blocks. The two infinitesimal conditions give

$$
X=\begin{pmatrix}P&Q\\-\overline Q&\overline P\end{pmatrix},\qquad P^*=-P,\quad Q^t=Q.
$$

The [skew-Hermitian matrix](../../../../../skew-hermitian-matrix.md) $P$ has $n^2$ real parameters; the complex symmetric matrix $Q$ has $n(n+1)/2$ complex parameters, hence $n(n+1)$ real parameters. Therefore

$$
\boxed{\dim_{\mathbb R}Sp(n)=n(2n+1).}
$$

For $n=1$, any two-by-two matrix satisfies $AJA^t=(\det A)J$, so the group is $SU(2)$. Explicitly,

$$
(a,b)\longmapsto\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix},\qquad |a|^2+|b|^2=1.
$$

The rows are orthonormal and the determinant is one; conversely unitarity and determinant one force this form. This is the [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md) parametrization. The map and its inverse, extraction of the first row, are smooth. Thus **$Sp(1)$ is diffeomorphic to $S^3$.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
