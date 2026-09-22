<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The zero [polynomial](../../../polynomial-split.md) belongs to $I_v$. If $f,g\in I_v$, linearity gives $(f-g)(T)v=0$. If $a\in K[X]$ and $f\in I_v$, [polynomial](../../../polynomial-split.md) evaluation obeys $(af)(T)=a(T)f(T)$, so $(af)(T)v=0$. Thus $I_v$ is an [ideal](../../../ideal.md) of the [polynomial ring](../../../polynomial-ring.md) $K[X]$.

The $n+1$ vectors $v,Tv,\ldots,T^nv$ are linearly dependent in the $n$-dimensional [vector space](../../../vector-space-split.md). Their dependence supplies a nonzero [polynomial](../../../polynomial-split.md) of [degree](../../../degree-of-a-polynomial.md) at most $n$ in $I_v$. Hence this [ideal](../../../ideal.md) is nonzero. A [polynomial](../../../polynomial-split.md) ring over a [field](../../../field.md) is a [Euclidean domain](../../../euclidean-domain.md) under [degree](../../../degree-of-a-polynomial.md), and every [ideal](../../../ideal.md) in a Euclidean domain is principal. It follows that $I_v=(m_v)$ for a nonzero [polynomial](../../../polynomial-split.md) $m_v$, which can be scaled uniquely to be monic.

For completeness, uniqueness follows because any two generators divide each other and hence differ by a nonzero constant; the monic normalization forces that constant to be one. Since $m_v$ divides the [polynomial](../../../polynomial-split.md) of [degree](../../../degree-of-a-polynomial.md) at most $n$ constructed above, its [degree](../../../degree-of-a-polynomial.md) is at most $n$. The generator characterization gives

$$
\boxed{m_v\mid f\quad\Longleftrightarrow\quad f\in I_v\quad\Longleftrightarrow\quad f(T)v=0.}
$$

This is the [minimal polynomial of a vector under a linear operator](../../../minimal-polynomial-of-a-vector-under-a-linear-operator.md). If $v=0$, the [ideal](../../../ideal.md) is the whole ring and the unique monic generator is the constant [polynomial](../../../polynomial-split.md) one.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2009](../../2009-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
