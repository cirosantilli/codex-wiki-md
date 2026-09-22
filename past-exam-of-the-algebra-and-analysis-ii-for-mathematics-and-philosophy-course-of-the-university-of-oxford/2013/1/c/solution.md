<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $p$ and $q$ are coprime, [Bézout's identity for polynomials](../../../../bezout-s-identity-for-polynomials.md) gives $a,b\in F[x]$ with $ap+bq=1$. For every $v\in V$,

$$
v=b(T)q(T)v+a(T)p(T)v.
$$

The first summand belongs to $U$: applying $p(T)$ gives $b(T)p(T)q(T)v=0$. The second belongs to $W$ by the same calculation. Here all [polynomials](../../../../polynomial-split.md) in $T$ commute, and $p(T)q(T)=f(T)=0$. Thus $V=U+W$.

If $v\in U\cap W$, both terms on the right of the identity vanish, so $v=0$. Therefore

$$
\boxed{V=U\oplus W.}
$$

Finally, $p(T)Tv=Tp(T)v=0$ whenever $v\in U$; hence $T(U)\subseteq U$. Replacing $p$ by $q$ proves $T(W)\subseteq W$. These are [invariant subspaces](../../../../invariant-subspace.md); this is the coprime-factor case of the [primary decomposition theorem for linear maps](../../../../primary-decomposition-theorem-for-linear-maps.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
