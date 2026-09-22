<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Construct compatible choices in the nested spaces, rather than choosing unrelated [orthonormal bases](../../../../../orthonormal-basis.md) for different $V_n$. Set $V_{-1}=\{0\}$ and define

$$
L_n=V_n\cap V_{n-1}^{\perp}.
$$

The [orthogonal complement](../../../../../orthogonal-complement.md) is taken for the [inner product](../../../../../inner-product-split.md) from part (i). Since $\dim V_n=n+1$ and $\dim V_{n-1}=n$, the space $L_n$ has dimension one and $V_n=V_{n-1}\oplus L_n$.

It is an [invariant subspace](../../../../../invariant-subspace.md). Indeed, if $v\in L_n$ and $u\in V_{n-1}$, part (ii) gives

$$
\langle u,Tv\rangle=\langle Tu,v\rangle=0,
$$

because $Tu\in V_{n-1}$. Also $Tv\in V_n$. Hence $Tv\in L_n$. Any nonzero vector in this one-dimensional space is consequently an [eigenvector](../../../../../eigenvector.md). Choose a unit vector $g_n\in L_n$. It has [polynomial degree](../../../../../degree-of-a-polynomial.md) exactly $n$: membership in $V_{n-1}$ would make it orthogonal to itself and thus zero. Part (iii) now supplies its [eigenvalue](../../../../../eigenvalue.md).

For $m<n$, $g_m\in V_{n-1}$ and $g_n\perp V_{n-1}$, so the choices are pairwise orthogonal. We have proved

$$
\boxed{\langle g_m,g_n\rangle=\delta_{mn},\qquad
\deg g_n=n,\qquad Tg_n=-2(n+1)g_n\quad(n\geq0).}
$$

An explicit compatible construction is the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) on $1,x,x^2,\ldots$:

$$
r_n=x^n-\sum_{j=0}^{n-1}\langle g_j,x^n\rangle g_j,
\qquad g_n=\frac{r_n}{\sqrt{\langle r_n,r_n\rangle}}.
$$

The leading term of $r_n$ is $x^n$, so it is never zero. This fixes the positive real leading coefficient and yields the normalized [Hermite polynomials](../../../../../hermite-polynomial.md). For example, the [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
g_0=\pi^{-1/4},\qquad
g_1=\sqrt2\,\pi^{-1/4}x,\qquad
g_2=\frac{2x^2-1}{\sqrt2\,\pi^{1/4}}.
$$

Every [polynomial](../../../../../polynomial-split.md) is a finite linear combination of these [eigenvectors](../../../../../eigenvector.md), since $g_0,\ldots,g_n$ form an [orthonormal basis](../../../../../orthonormal-basis.md) of $V_n$ for each $n$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
