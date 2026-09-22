<h1 id="18f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use first-kind [Chebyshev polynomials](../../../../../../chebyshev-polynomial.md) $T_j$, characterized by $T_j(\cos\theta)=\cos(j\theta)$. Substituting $x=\cos\theta$ converts the weighted [inner product](../../../../../../inner-product.md) into $\int_0^\pi g(\cos\theta)h(\cos\theta)d\theta$. Hence these [polynomials](../../../../../../polynomial-split.md) are [orthogonal](../../../../../../orthogonal-vectors.md), with squared [norms](../../../../../../norm.md) $\pi$ for $j=0$ and $\pi/2$ for $j\geq1$.

For the specified [function](../../../../../../function-split.md), $f(\cos\theta)=\sin\theta$. Its constant projection coefficient is $\pi^{-1}\int_0^\pi\sin\theta\,d\theta=2/\pi$. For $j\geq1$ the coefficient is $(2/\pi)\int_0^\pi\sin\theta\cos(j\theta)d\theta$. Symmetry about $\pi/2$ makes it zero for odd $j$. For $j=2m$, the product-to-sum identity gives

$$
\int_0^\pi\sin\theta\cos(2m\theta)d\theta
=\frac1{1+2m}+\frac1{1-2m}=\frac2{1-4m^2}.
$$

Therefore the [Chebyshev projection of a semicircle](../../../../../../chebyshev-projection-of-a-semicircle.md) is

$$
\boxed{p_n(x)=\frac2\pi-\frac4\pi\sum_{m=1}^{\lfloor n/2\rfloor}\frac{T_{2m}(x)}{4m^2-1}.}
$$

In particular the best degree-at-most-$n$ [polynomial](../../../../../../polynomial-split.md) is even, so for odd $n$ its actual degree is at most $n-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18F](../../18f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
