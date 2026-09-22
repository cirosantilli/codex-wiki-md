<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

First work over a field of characteristic different from two. If a nonzero [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) had $\phi(v,v)=0$ for every [vector](../../../../../vector.md), polarization would give

$$
2\phi(u,v)=\phi(u+v,u+v)-\phi(u,u)-\phi(v,v)=0,
$$

a contradiction. Hence choose $e$ with $\phi(e,e)\ne0$. Every $v$ decomposes uniquely as

$$
v=\frac{\phi(v,e)}{\phi(e,e)}e+\left(v-\frac{\phi(v,e)}{\phi(e,e)}e\right),
$$

with the second summand orthogonal to $e$. Induct on the [orthogonal complement](../../../../../orthogonal-complement.md) to obtain a diagonal basis. If the restricted form becomes zero, any basis of that remaining space completes the diagonalization. In this basis the [rank of a quadratic form](../../../../../rank-of-a-quadratic-form.md) is exactly the number of nonzero diagonal coefficients; the remaining basis [vectors](../../../../../vector.md) span its [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md).

Over the reals, rescale the nonzero basis [vectors](../../../../../vector.md) so the diagonal entries are $p$ copies of $+1$, $q$ copies of $-1$ and $z=n-p-q$ zeros. Define the [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) by $\sigma=p-q$, so $r=p+q$. To prove it is basis independent, note that $p$ is the largest dimension of a [linear subspace](../../../../../vector-subspace.md) on which the form is [positive-definite](../../../../../positive-definite-bilinear-form.md). The positive coordinate [linear subspace](../../../../../vector-subspace.md) attains dimension $p$; on any other positive [linear subspace](../../../../../vector-subspace.md), projection to those positive coordinates is injective, since its kernel has nonpositive quadratic value. Thus its dimension is at most $p$. The same argument for the negative form characterizes $q$. This proves [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) and that the signature is well-defined.

Let $e_i$ and $f_i$ be positive and negative normalized basis [vectors](../../../../../vector.md), and let $Z$ be the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md). The span of $Z$ and $e_i+f_i$ for $1\leq i\leq\min(p,q)$ is a [totally isotropic subspace](../../../../../totally-isotropic-subspace.md): all mutual bilinear pairings vanish. Its dimension is $z+\min(p,q)$. Conversely, project any [totally isotropic subspace](../../../../../totally-isotropic-subspace.md) $U$ to the nondegenerate positive-plus-negative quotient. The projected [linear subspace](../../../../../vector-subspace.md) is still null, and its projections to both the positive and negative coordinate spaces are injective: a [vector](../../../../../vector.md) with one component zero would have strictly signed quadratic value unless it vanished. Its dimension is therefore at most $\min(p,q)$, while the kernel of the quotient map on $U$ has dimension at most $z$. Hence

$$
\boxed{\max\dim U=z+\min(p,q)=n-\frac{r+|\sigma|}{2}}.
$$

This proves both construction and sharpness of the [maximum dimension of a totally isotropic subspace](../../../../../maximum-dimension-of-a-totally-isotropic-subspace.md).

For the five-variable example, the symmetric coefficient [matrix](../../../../../matrix.md) is

$$
A=\begin{pmatrix}
0&1&0&0&1\\1&0&1&0&0\\0&1&0&1&0\\0&0&1&0&1\\1&0&0&1&0
\end{pmatrix}.
$$

Its cyclic structure makes the [vectors](../../../../../vector.md) $(1,\zeta^k,\zeta^{2k},\zeta^{3k},\zeta^{4k})$, $\zeta=e^{2\pi i/5}$, [eigenvectors](../../../../../eigenvector.md) with [eigenvalues](../../../../../eigenvalue.md) $\zeta^k+\zeta^{-k}=2\cos(2\pi k/5)$. Thus the [eigenvalues](../../../../../eigenvalue.md) are

$$
2,\qquad \frac{\sqrt5-1}{2}\ \text{(twice)},\qquad -\frac{\sqrt5+1}{2}\ \text{(twice)}.
$$

Their product is $2$, and three are positive and two negative. Therefore

$$
\boxed{\det A=2,\qquad r=5,\qquad\sigma=1}.
$$

The real and imaginary parts of each conjugate pair of [eigenvectors](../../../../../eigenvector.md) give the corresponding real two-dimensional [eigenspaces](../../../../../eigenspace.md), consistent with the real inertia calculation.

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
