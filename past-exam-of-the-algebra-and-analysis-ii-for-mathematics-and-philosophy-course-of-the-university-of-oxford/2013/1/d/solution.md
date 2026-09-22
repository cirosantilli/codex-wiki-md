<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $m_1,m_2$ for the [minimal polynomials](../../../../minimal-polynomial.md) of the two [restrictions](../../../../restriction-mathematics.md). Since $p(T)$ vanishes on $U$ and $q(T)$ vanishes on $W$, part (b) gives

$$
m_1\mid p,\qquad m_2\mid q.
$$

Hence $m_1,m_2$ are coprime. By the direct-sum decomposition, a [polynomial](../../../../polynomial-split.md) annihilates $T$ exactly when it annihilates both [restrictions](../../../../restriction-mathematics.md), which happens exactly when it is divisible by both $m_1$ and $m_2$. Consequently

$$
m_T=\operatorname{lcm}(m_1,m_2)=m_1m_2.
$$

If $m_1=p$ and $m_2=q$, this immediately gives $m_T=pq=f$. Conversely, if $m_T=pq$, the [monic polynomials](../../../../monic-polynomial.md) $p/m_1$ and $q/m_2$ have product one, so each is one. Thus

$$
\boxed{m_T=pq\iff m_{T|_U}=p\text{ and }m_{T|_W}=q.}
$$

This also handles a zero summand, whose [minimal polynomial](../../../../minimal-polynomial.md) is one; a nonconstant factor cannot be its [minimal polynomial](../../../../minimal-polynomial.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
