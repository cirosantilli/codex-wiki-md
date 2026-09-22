<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [matrix trace](../../../../matrix-trace.md) is $\operatorname{Tr}A=\sum_iA_{ii}$. Expanding the [matrix products](../../../../matrix-product.md) gives $\operatorname{Tr}(AB)=\sum_{i,j}A_{ij}B_{ji}=\sum_{j,i}B_{ji}A_{ij}=\operatorname{Tr}(BA)$. Thus the [cyclic property of the trace](../../../../cyclic-property-of-the-trace.md) gives zero [trace](../../../../matrix-trace.md) to every [commutator](../../../../commutator.md). If $AB-BA=I$, taking the [trace](../../../../matrix-trace.md) would give $0=n$, impossible for positive finite $n$ over the real or complex [field](../../../../field.md).

For real $A,B$, let $p(\lambda)=\det(A+\lambda B)$, a real [polynomial](../../../../polynomial-split.md) of degree at most $n$. Since $p(i)=\det C\ne0$, it is not the zero [polynomial](../../../../polynomial-split.md). It has at most finitely many real [roots of a polynomial](../../../../root-of-a-polynomial.md), so $A+\lambda B$ is an [invertible matrix](../../../../invertible-matrix.md) for some real $\lambda$, in fact for all but finitely many.

Finally write the invertible intertwiner as $R=A+iB$. The relation $PR=RQ$ and the reality of $P,Q$ give $PA=AQ$ and $PB=BQ$. Choose a real $\lambda$ for which $S=A+\lambda B$ is invertible. Then $PS=SQ$, so $P=SQS^{-1}$. This proves that [complex similarity of real matrices implies real similarity](../../../../complex-similarity-of-real-matrices-implies-real-similarity.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
