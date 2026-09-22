<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [adjoint on an inner product space](../../../adjoint-on-an-inner-product-space.md) $\alpha^*:V\to V$ is characterized by

$$
\langle\alpha v,w\rangle=\langle v,\alpha^*w\rangle\qquad(v,w\in V).
$$

Here is a finite-dimensional construction that supplies every required [basis](../../../basis.md) fact. If $v_1,\ldots,v_n$ is any [basis](../../../basis.md), its coordinate [linear functionals](../../../linear-functional.md) form a [basis](../../../basis.md) of $V^*$: a [linear functional](../../../linear-functional.md) is uniquely specified by its values on these $n$ [vectors](../../../vector.md). Hence $\dim V^*=n$. The [linear map](../../../linear-map.md)

$$
J:V\to V^*,\qquad J(w)(v)=\langle v,w\rangle
$$

is [injective](../../../injective-function.md), because $J(w)=0$ implies $\langle w,w\rangle=0$, and [positive definiteness](../../../positive-definiteness.md) implies $w=0$. Equal [dimensions](../../../dimension-vector-space.md) make $J$ an [linear isomorphism](../../../linear-isomorphism.md). If $\alpha'$ is the [dual map](../../../transpose-of-a-linear-map.md), then

$$
\alpha^*=J^{-1}\alpha'J.
$$

This establishes existence and [linearity](../../../linearity.md). If two possible [vectors](../../../vector.md) $u,w$ represent the same [linear functional](../../../linear-functional.md) through the [inner product](../../../inner-product-split.md), then $J(u-w)=0$, so $u=w$. Applied to every argument, this proves uniqueness of the [adjoint on an inner product space](../../../adjoint-on-an-inner-product-space.md).

For [linear maps](../../../linear-map.md) $S,T$, two applications of the defining [inner product](../../../inner-product-split.md) identity give

$$
\langle STv,w\rangle=\langle Tv,S^*w\rangle=\langle v,T^*S^*w\rangle.
$$

Uniqueness therefore gives $(ST)^*=T^*S^*$. Likewise $(S+T)^*=S^*+T^*$, $(cT)^*=cT^*$ for real $c$, and $I^*=I$. An [induction](../../../mathematical-induction.md) gives $(\alpha^n)^*=(\alpha^*)^n$, and applying additivity to a [polynomial](../../../polynomial-split.md) with real coefficients gives

$$
\boxed{f(\alpha)^*=f(\alpha^*).}
$$

Symmetry of the real [inner product](../../../inner-product-split.md) also gives $(\alpha^*)^*=\alpha$. If $m$ is the [minimal polynomial](../../../minimal-polynomial.md) of $\alpha$, the displayed identity gives $m(\alpha^*)=0$, so the [minimal polynomial](../../../minimal-polynomial.md) of $\alpha^*$ divides $m$. Applying the same argument to $\alpha^*$ gives reverse divisibility. Both [polynomials](../../../polynomial-split.md) are [monic](../../../monic-polynomial.md), hence **their minimal polynomials are equal**.

The distinct [eigenvalues](../../../eigenvalue.md) are exactly the roots of the [minimal polynomial](../../../minimal-polynomial.md) in the chosen [field](../../../field.md). An [eigenvector](../../../eigenvector.md) $v$ with [eigenvalue](../../../eigenvalue.md) $\lambda$ satisfies $m(\alpha)v=m(\lambda)v$, so $m(\lambda)=0$. Conversely, if $m(X)=(X-\lambda)q(X)$ and $\alpha-\lambda I$ were a [linear isomorphism](../../../linear-isomorphism.md), then $m(\alpha)=0$ would imply $q(\alpha)=0$, contradicting minimal degree. Thus $\alpha-\lambda I$ is not [injective](../../../injective-function.md), giving an [eigenvector](../../../eigenvector.md). It follows that $\alpha$ and $\alpha^*$ have **the same distinct eigenvalues**. This includes the complex [eigenvalues](../../../eigenvalue.md) after [complexification of a real vector space](../../../complexification-of-a-real-vector-space.md); over the real [field](../../../field.md) it states equality of their real [eigenvalues](../../../eigenvalue.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
