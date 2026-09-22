<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $d=\dim V$. A [cyclic vector](../../../../cyclic-vector.md) for $S$ is a vector $v$ whose successive iterates span $V$; equivalently, when $d>0$,

$$
v,Sv,\ldots,S^{d-1}v
$$

are a [basis](../../../../basis.md). The equivalence follows because the first linear dependence in the iterates makes their preceding span invariant under $S$, so no later iterate can enlarge it.

In this basis there are unique coefficients $c_0,\ldots,c_{d-1}$ with $S^dv=-\sum_{j<d}c_jS^jv$. Put $f(t)=t^d+\sum_{j<d}c_jt^j$. Then $f(S)v=0$, and commutation with powers of $S$ gives $f(S)S^jv=S^jf(S)v=0$. Therefore $f(S)$ kills an entire basis and is the zero map. No nonzero polynomial of degree less than $d$ annihilates $v$, because that would be a linear dependence of the displayed basis. Thus $m_S=f$.

The matrix of $S$ in the cyclic basis is the [companion matrix](../../../../companion-matrix.md) $C(f)$ with ones on its subdiagonal and last column $(-c_0,\ldots,-c_{d-1})^{\mathsf T}$. Expanding $\det(tI-C(f))$ along its last column gives

$$
c_0+c_1t+\cdots+c_{d-2}t^{d-2}+(t+c_{d-1})t^{d-1}=f(t):
$$

the cofactors are $1,t,\ldots,t^{d-1}$. This proves the [characteristic polynomial of a companion matrix](../../../../characteristic-polynomial-of-a-companion-matrix.md) formula here. Hence

$$
\boxed{m_S(t)=c_S(t)=f(t).}
$$

This proves that a [cyclic operator has equal minimal and characteristic polynomials](../../../../cyclic-operator-has-equal-minimal-and-characteristic-polynomials.md). If $V=\{0\}$, both polynomials are one by convention, so the equality remains valid.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
