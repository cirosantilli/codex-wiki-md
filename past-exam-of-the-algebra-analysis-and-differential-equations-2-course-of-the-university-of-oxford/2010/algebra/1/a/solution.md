<h1 id="algebra/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $n=\dim V$. If $Rv=\lambda v$ with $v\ne0$, then $0=R^av=\lambda^av$, hence $\lambda=0$. The [characteristic polynomial](../../../../../characteristic-polynomial.md) splits over $\mathbb C$ and has degree $n$, so

$$
\boxed{\operatorname{spec}(R)=\{0\},\qquad\chi_R(t)=t^n.}
$$

There is indeed an [eigenvector](../../../../../eigenvector.md) for the [eigenvalue](../../../../../eigenvalue.md) zero: a nonzero [vector](../../../../../vector.md) in the last nonzero [image](../../../../../image-of-a-function.md) of $R$ lies in its [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md). For the bound, choose $v$ with $R^{a-1}v\ne0$, using minimality. The vectors $v,Rv,\ldots,R^{a-1}v$ are [linearly independent](../../../../../linear-independence.md). Otherwise choose the least $j$ with nonzero coefficient in a relation and apply $R^{a-1-j}$; only its nonzero multiple of $R^{a-1}v$ survives, a contradiction. Therefore $\boxed{a\le n}$.

## ↑ Ancestors (13)

1. [A](../a.md)
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
