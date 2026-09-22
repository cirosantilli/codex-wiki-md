<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Polynomial functions](../../../../polynomial-function.md) are regular, giving an [injective](../../../../injective-function.md) map $A(X)\hookrightarrow\mathcal O_X(X)$; [injectivity](../../../../injective-function.md) follows from quotienting by the full [vanishing ideal](../../../../vanishing-ideal.md). To prove [surjectivity](../../../../surjective-function.md), let $f$ be globally regular and consider the denominator [ideal](../../../../ideal.md)

$$
J=\{g\in A(X):gf\text{ is a polynomial function on }X\}.
$$

It is an [ideal](../../../../ideal.md) because sums and [polynomial](../../../../polynomial-split.md) multiples preserve this property.

Fix $p\in X$. Locally $f=a/b$ on a [neighbourhood](../../../../neighbourhood-mathematics.md) $V$ of $p$, with $b$ nonzero there. Principal affine opens form a [basis](../../../../basis.md), so choose $h\in A(X)$ with $h(p)\neq0$ and $D(h)\subseteq V$. Then

$$
(hb)f=ha
$$

as functions on all of $X$: on $D(h)$ it follows from the local fraction, and off $D(h)$ both sides vanish because $h=0$. Hence $hb\in J$ and $(hb)(p)\neq0$.

Thus $J$ has no common zero on $X$. By the weak Nullstellensatz for $A(X)$, every proper [ideal](../../../../ideal.md) lies in a [maximal ideal](../../../../maximal-ideal.md) belonging to a [point](../../../../point-geometry.md) of $X$; therefore $J$ cannot be proper. We get $1\in J$, so $f$ itself is [polynomial](../../../../polynomial-split.md). This proves

$$
\boxed{\mathcal O_X(X)\cong A(X).}
$$

The argument works for reducible [affine varieties](../../../../affine-algebraic-set.md) as well: it uses functions and denominator [ideals](../../../../ideal.md) rather than assuming a single [fraction field](../../../../field-of-fractions.md).

This is the [denominator ideal proof for global regular functions](../../../../denominator-ideal-proof-for-global-regular-functions.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
