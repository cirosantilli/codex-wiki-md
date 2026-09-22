<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [minimal polynomial](../../../minimal-polynomial.md) $m_T$ is the unique monic polynomial of least degree with $m_T(T)=0$. Existence follows from a linear dependence among powers of $T$ in the finite-dimensional vector space $\operatorname{End}(V)$; polynomial division proves uniqueness and that it divides every annihilating polynomial. The [characteristic polynomial](../../../characteristic-polynomial.md) is $\chi_T(t)=\det(tI-[T]_{\mathcal B})$, independent of basis because a change of basis conjugates the matrix.

Write

$$
T^nv=-a_0v-a_1Tv-\cdots-a_{n-1}T^{n-1}v.
$$

In the cyclic basis, the [companion matrix](../../../companion-matrix.md) is

$$
C=\begin{pmatrix}
0&0&\cdots&0&-a_0\\
1&0&\cdots&0&-a_1\\
0&1&\cdots&0&-a_2\\
\vdots&&\ddots&\vdots&\vdots\\
0&0&\cdots&1&-a_{n-1}
\end{pmatrix}.
$$

For $q(t)=t^n+a_{n-1}t^{n-1}+\cdots+a_0$, the displayed vector relation gives $q(T)v=0$. Polynomial evaluation commutes with $T$, so $q(T)T^jv=T^jq(T)v=0$ for every basis vector. Thus $q(T)=0$.

No nonzero polynomial of degree below $n$ can annihilate $T$, since applying it to the [cyclic vector](../../../cyclic-vector.md) $v$ would contradict independence of $v,Tv,\ldots,T^{n-1}v$. Hence $m_T=q$. Finally, direct expansion of $\det(tI-C)$, or induction along the last column, gives $\chi_T(t)=t^n+a_{n-1}t^{n-1}+\cdots+a_0=q(t)$. Therefore

$$
\boxed{m_T=\chi_T=q.}
$$

The argument computes the determinant and annihilator directly and does not invoke the [Cayley-Hamilton theorem](../../../cayley-hamilton-theorem-split.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
