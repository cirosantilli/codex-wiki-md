# Gaussian polynomial operator

↑ **Parent:** [Hermite polynomial](hermite-polynomial.md)

On $\mathbb C[x]$, equip [polynomials](polynomial-split.md) with the [inner product](inner-product-split.md)

$$
\langle f,g\rangle=\int_{-\infty}^{\infty}\overline{f(x)}g(x)e^{-x^2}\,dx.
$$

The [linear operator](linear-operator.md)

$$
Tf=\frac{d}{dx}\left(e^{x^2}\frac{d}{dx}(e^{-x^2}f)\right)
=f''-2xf'-2f
$$

preserves the space $V_n$ of [polynomials](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) at most $n$. [Integration by parts](integration-by-parts.md), whose boundary terms vanish by Gaussian decay, gives

$$
\langle Tf,g\rangle=-\langle f',g'\rangle-2\langle f,g\rangle
=\langle f,Tg\rangle.
$$

Thus $T$ equals its [adjoint on an inner product space](adjoint-on-an-inner-product-space.md). If a nonzero [polynomial](polynomial-split.md) of degree $n$ is an [eigenvector](eigenvector.md), its leading coefficient forces its [eigenvalue](eigenvalue.md) to be $-2(n+1)$.

One can construct all these [eigenvectors](eigenvector.md) without solving a [differential equation](differential-equation-split.md). The one-dimensional space $L_n=V_n\cap V_{n-1}^{\perp}$ is invariant: for $u\in V_{n-1}$ and $v\in L_n$, the displayed identity gives $\langle u,Tv\rangle=\langle Tu,v\rangle=0$. Its unit vector of positive real leading coefficient is therefore an [eigenvector](eigenvector.md) of degree $n$. These choices are exactly the [Gram-Schmidt process](gram-schmidt-process.md) applied to $1,x,x^2,\ldots$, producing normalized [Hermite polynomials](hermite-polynomial.md). Their first three members are

$$
g_0=\pi^{-1/4},\qquad g_1=\sqrt2\pi^{-1/4}x,\qquad
g_2=\frac{2x^2-1}{\sqrt2\pi^{1/4}}.
$$

Every [polynomial](polynomial-split.md) is a finite linear combination of these orthonormal [eigenvectors](eigenvector.md).

## ↑ Ancestors (7)

1. [Hermite polynomial](hermite-polynomial.md)
2. [Orthogonal polynomial](orthogonal-polynomial-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Adjoint on an inner product space](adjoint-on-an-inner-product-space.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2017/3/b/ii/solution.md)
