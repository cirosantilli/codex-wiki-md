<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

A [linear operator](../../../../../linear-operator.md) $\alpha$ on a real inner-product space is [self-adjoint](../../../../../self-adjoint-operator.md) when

$$
\langle\alpha v,w\rangle=\langle v,\alpha w\rangle
$$

for all $v,w$.

To prove the [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md), first note that the continuous [quadratic function](../../../../../quadratic-function.md) $\langle\alpha v,v\rangle$ has a maximum on the unit sphere. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equation at a maximizing [vector](../../../../../vector.md) $v$ gives $\alpha v=\lambda v$, so $\alpha$ has a real unit [eigenvector](../../../../../eigenvector.md). Its orthogonal complement is invariant because

$$
\langle\alpha w,v\rangle=\langle w,\alpha v\rangle
=\lambda\langle w,v\rangle=0.
$$

Induction on the dimension supplies an orthonormal eigenbasis of that complement and hence of $V$.

For $f\ne0$,

$$
\langle f,f\rangle=\int_0^\infty f(x)^2e^{-x}\,dx>0,
$$

while symmetry and bilinearity are immediate, so the displayed formula defines an [inner product](../../../../../inner-product.md) on $P_n$. Since

$$
e^{-x}\alpha(f)
=\bigl(xe^{-x}f'(x))',
$$

[integration by parts](../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\langle\alpha f,g\rangle
&=\left[gxe^{-x}f'\right]_0^\infty
-\int_0^\infty x e^{-x}f'g'\,dx\\
&=\langle f,\alpha g\rangle.
\end{aligned}
$$

The boundary term vanishes for [polynomials](../../../../../polynomial-split.md), proving that $\alpha$ is self-adjoint.

On the monomial $x^k$,

$$
\alpha(x^k)=-kx^k+k^2x^{k-1}.
$$

Thus the [matrix](../../../../../matrix.md) of $\alpha$ in the monomial [basis](../../../../../basis.md) is triangular with diagonal

$$
0,-1,-2,\ldots,-n.
$$

These are therefore its [eigenvalues](../../../../../eigenvalue.md). For $n=2$, corresponding [eigenvectors](../../../../../eigenvector.md) are

$$
\boxed{
1,\qquad x-1,\qquad x^2-4x+2
}
$$

for [eigenvalues](../../../../../eigenvalue.md) $0,-1,-2$, respectively. They are the first [Laguerre polynomials](../../../../../laguerre-polynomial.md) up to normalization, as described by the [Laguerre differential operator on polynomials](../../../../../laguerre-differential-operator-on-polynomials.md).

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
