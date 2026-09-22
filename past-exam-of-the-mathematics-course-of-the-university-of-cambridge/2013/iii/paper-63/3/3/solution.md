<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The appropriate bounded-operator formulation uses the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md)

$$
H=H_0^1(-1,1),\qquad (u,v)_H=\int_{-1}^1u'v'\,dx.
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) makes this a [Hilbert space](../../../../../../hilbert-space-split.md) norm equivalent to the usual $H^1$ norm, and the zero endpoint traces encode the [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md). Under the usual regular-coefficient assumptions, for example continuous $p,q$ on the closed interval with $p>0$ and $q\geq0$, set

$$
a(u,v)=\int_{-1}^1\bigl(pu'v'+quv\bigr)\,dx.
$$

If $p_*=\min p>0$, then [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [Poincaré inequality](../../../../../../poincare-inequality.md) give

$$
|a(u,v)|\leq(\|p\|_\infty+C_P^2\|q\|_\infty)\|u\|_H\|v\|_H,
\qquad a(v,v)\geq p_*\|v\|_H^2.
$$

By the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md), a unique [bounded linear operator](../../../../../../continuous-linear-operator.md) $T:H\to H$ satisfies $(Tu,v)_H=a(u,v)$. Symmetry of $a$ makes $T$ [self-adjoint](../../../../../../self-adjoint-operator.md), and the lower bound makes it elliptic and **uniformly positive definite**. The differential expression in the question is represented weakly by $a$: for smooth functions, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_{-1}^1\bigl[-(pu')'+qu\bigr]v\,dx=a(u,v),
$$

with the boundary term zero. A forcing $f\in L^2$ becomes the bounded functional $v\mapsto\int fv$, or its Riesz representative in $H$.

Equivalently, for sufficiently smooth coefficients one may realize the differential operator itself on $L^2(-1,1)$ with domain $H^2\cap H_0^1$. Its regular [Sturm-Liouville operator](../../../../../../sturm-liouville-operator.md) realization is [self-adjoint](../../../../../../self-adjoint-operator.md) and

$$
\langle Lu,u\rangle_{L^2}=\int_{-1}^1\bigl(p|u'|^2+q|u|^2\bigr)\,dx>0\quad(u\ne0).
$$

This realization is an unbounded operator, so it should not be confused with the bounded weak operator $T$ used above.

The PDF states sign conditions without coefficient regularity. If only $p>0$ almost everywhere and $p,q$ are bounded, the same form is still bounded and strictly positive: a zero energy would force $u'=0$ almost everywhere and the zero traces force $u=0$. Uniform ellipticity, however, requires a positive lower bound. For instance $p(x)=x^2$ for $x\ne0$, $p(0)=1$, and $q=0$ satisfy literal pointwise positivity. Derivatives of unit $L^2$ norm supported in $(\varepsilon,2\varepsilon)$ and of integral zero define functions in $H_0^1$, with energy at most $4\varepsilon^2$. Thus pointwise positivity without regularity does not imply coercivity in this $H$ norm. These distinctions supply the precise regularity and operator domain behind the intended positive-definiteness proof.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
