<h1 id="algebra/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [polynomials](../../../../../polynomial-split.md) $t^c$ and $(t-1)^d$ are [coprime](../../../../../coprime-integers.md). [Bézout's identity](../../../../../bezout-s-identity.md) gives [polynomials](../../../../../polynomial-split.md) $u,v$ with $u(t)t^c+v(t)(t-1)^d=1$. Set

$$
V_0=\ker T^c,\qquad V_1=\ker(T-I)^d.
$$

For every $x$, the decomposition

$$
x=v(T)(T-I)^dx+u(T)T^cx
$$

has first summand in $V_0$ and second in $V_1$, since $T^c(T-I)^d=0$ and [polynomial](../../../../../polynomial-split.md) expressions in $T$ commute. If $x$ belongs to both [kernels](../../../../../kernel-of-a-linear-map-split.md), the same Bézout identity gives $x=0$. Thus $V=V_0\oplus V_1$. Both [vector subspaces](../../../../../vector-subspace.md) are [invariant](../../../../../invariant-mathematics.md) under $T$.

On $V_0$, the restriction of $T$ is [nilpotent](../../../../../nilpotent-linear-map.md); on $V_1$, the restriction of $T-I$ is [nilpotent](../../../../../nilpotent-linear-map.md). Apply (b) separately, then concatenate the two [bases](../../../../../basis.md). This yields

$$
\boxed{[T]=\begin{pmatrix}A&0\\0&I+N\end{pmatrix},}
$$

where $A,N$ are [strictly upper triangular](../../../../../strictly-upper-triangular-matrix.md). Empty blocks are allowed if one subspace is zero. In particular $C=I+N$ has precisely the required diagonal.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Algebra](../../../algebra.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
