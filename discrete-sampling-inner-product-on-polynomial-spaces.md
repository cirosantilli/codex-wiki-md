# Discrete sampling inner product on polynomial spaces

↑ **Parent:** [Inner product](inner-product-split.md)

Let $P_n(\mathbb R)$ be the [vector space](vector-space-split.md) of real [polynomials](polynomial-split.md) of [degree of a polynomial](degree-of-a-polynomial.md) at most $n$. Choose $n+1$ distinct real sample points $t_0,\ldots,t_n$ and positive real weights $w_0,\ldots,w_n$. Then

$$
\langle f,g\rangle=\sum_{j=0}^{n}w_jf(t_j)g(t_j)
$$

is an [inner product](inner-product-split.md). Symmetry and [bilinearity](bilinearity.md) follow from [linearity](linearity.md) of [polynomial evaluation](polynomial-evaluation.md). Its value at $(f,f)$ is nonnegative, and equality forces all $f(t_j)=0$. By the [root bound for a polynomial](lagrange-root-bound-over-a-field.md), a nonzero [polynomial](polynomial-split.md) of [degree of a polynomial](degree-of-a-polynomial.md) at most $n$ cannot vanish at $n+1$ distinct points. Thus the form has [positive definiteness](positive-definiteness.md).

Equivalently, the [polynomial evaluation map on a finite point set](polynomial-evaluation-map-on-a-finite-point-set.md) identifies $P_n(\mathbb R)$ with $\mathbb R^{n+1}$, equipped with a [weighted Euclidean inner product](weighted-euclidean-inner-product.md). Too few sample points destroy [positive definiteness](positive-definiteness.md): if the distinct points number at most $n$, the nonzero [polynomial](polynomial-split.md) $\prod_j(x-t_j)$ lies in $P_n(\mathbb R)$ and has zero sampled squared [norm](norm.md).

For three equally weighted samples at $-1,0,1$, an [orthonormal basis](orthonormal-basis.md) is

$$
1,\qquad\sqrt{\frac32}\,x,\qquad\frac{3x^2-2}{\sqrt2}.
$$

This construction gives a finite sampling version of [orthogonal polynomials](orthogonal-polynomial-split.md) and permits exact [Gram-Schmidt orthogonalization](gram-schmidt-process.md) using only finitely many evaluations.

## ↑ Ancestors (6)

1. [Inner product](inner-product-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/4/a/solution.md)
