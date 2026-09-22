<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A real [Lie group](../../../../../lie-group.md) is a group $G$ equipped with a finite-dimensional real [smooth manifold](../../../../../smooth-manifold.md) structure, conventionally Hausdorff and second countable, for which multiplication $G\times G\to G$ and inversion $G\to G$ are smooth.

Its [tangent space](../../../../../tangent-space.md) at the identity $e$ is defined by smooth curves through $e$: two curves represent the same tangent vector when their derivatives in a local chart agree at zero. For $X\in T_eG$, left translation $L_g(h)=gh$ determines the [left-invariant vector field](../../../../../left-invariant-vector-field.md)

$$
X^L(g)=(dL_g)_eX.
$$

The commutator of these derivations on smooth functions is another [left-invariant vector field](../../../../../left-invariant-vector-field.md), so define the [Lie bracket](../../../../../lie-bracket.md)

$$
\boxed{[X,Y]=[X^L,Y^L](e),\qquad\operatorname{Lie}(G)=T_eG.}
$$

This construction supplies the [Lie algebra](../../../../../lie-algebra-split.md) structure. In a [Matrix Lie group](../../../../../matrix-lie-group.md), $X^L(g)=gX$ and differentiating the two fields gives $[X,Y]=XY-YX$.

For the [special linear group](../../../../../special-linear-group.md), differentiate the [determinant](../../../../../determinant.md) along a curve $g(t)$ through $I$. Expansion of the [determinant](../../../../../determinant.md), or its differential $D\det_A(H)=\det(A)\operatorname{tr}(A^{-1}H)$, gives

$$
\left.\frac d{dt}\det(I+tX)\right|_{t=0}=\operatorname{tr}X.
$$

The [determinant](../../../../../determinant.md) differential is surjective at $I$, so the level set $\det=1$ has [tangent space](../../../../../tangent-space.md) equal to its differential's [kernel](../../../../../kernel-of-a-linear-map.md). Equivalently, every tangent matrix has zero [trace](../../../../../matrix-trace.md), and every zero-trace matrix supplies a curve $e^{tX}$ of [determinant](../../../../../determinant.md) $e^{t\operatorname{tr}X}=1$. Hence

$$
\boxed{\operatorname{Lie}(\mathrm{SL}_n(\mathbb R))=\mathfrak{sl}_n(\mathbb R)=\{X:\operatorname{tr}X=0\},}
$$

with the matrix [commutator](../../../../../commutator.md) bracket. The same calculation over $\mathbb C$ gives the complex [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_n(\mathbb C)$; as a real group, the complex group has that space viewed as a real [Lie algebra](../../../../../lie-algebra-split.md).

The [matrix exponential](../../../../../matrix-exponential.md) is the everywhere-convergent series

$$
\boxed{\exp X=\sum_{k=0}^\infty\frac{X^k}{k!},\qquad X\in\mathfrak{gl}_n,}
$$

whose inverse matrix is $\exp(-X)$. The [matrix logarithm](../../../../../matrix-logarithm.md) is locally defined near $I$ by

$$
\boxed{\log(I+A)=\sum_{k=1}^\infty\frac{(-1)^{k+1}}kA^k,\qquad\|A\|<1.}
$$

These maps are inverse on suitable neighbourhoods of zero and $I$, giving a [logarithmic chart of a matrix Lie group](../../../../../logarithmic-chart-of-a-matrix-lie-group.md). A logarithm is not a globally single-valued inverse of the exponential.

Every invertible complex matrix nevertheless has at least one [matrix logarithm](../../../../../matrix-logarithm.md). Put it in [Jordan normal form](../../../../../jordan-normal-form.md). For a block $J=\lambda I+N$, $\lambda\ne0$ and $N^s=0$, choose any complex scalar logarithm $\ell$ of $\lambda$ and set

$$
L=\ell I+\sum_{k=1}^{s-1}\frac{(-1)^{k+1}}k\left(\frac N\lambda\right)^k.
$$

The finite logarithm and exponential identities in the nilpotent variable give $e^L=\lambda(I+N/\lambda)=J$. Combine the blocks and conjugate back. Thus **the exponential map is surjective on** $\mathrm{GL}_n(\mathbb C)$, by [existence of a logarithm for every invertible complex matrix](../../../../../existence-of-a-logarithm-for-every-invertible-complex-matrix.md).

A connected counterexample is $\mathrm{SL}_2(\mathbb R)$. It is connected: [polar decomposition of an invertible real matrix](../../../../../polar-decomposition-of-an-invertible-real-matrix.md) writes each element as $KP$, with $K\in\mathrm{SO}(2)$ and $P$ positive definite symmetric of [determinant](../../../../../determinant.md) one; $\mathrm{SO}(2)$ is connected and $P$ is connected to $I$ through $P^t$.

But $g=\operatorname{diag}(-2,-1/2)$ belongs to this group and is not $e^X$ for any real $X$. Such an $X$ would commute with $e^X=g$. Since $g$ has two distinct real [eigenvalues](../../../../../eigenvalue.md), direct commutation makes $X$ a real [diagonal matrix](../../../../../diagonal-matrix.md). Its exponential has positive diagonal entries, a contradiction. Therefore

$$
\boxed{\exp:\mathfrak{sl}_2(\mathbb R)\longrightarrow\mathrm{SL}_2(\mathbb R)\text{ is not surjective}.}
$$

This is an [exponential-surjectivity obstruction from distinct negative eigenvalues](../../../../../exponential-surjectivity-obstruction-from-distinct-negative-eigenvalues.md); connectedness does not eliminate the obstruction.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
