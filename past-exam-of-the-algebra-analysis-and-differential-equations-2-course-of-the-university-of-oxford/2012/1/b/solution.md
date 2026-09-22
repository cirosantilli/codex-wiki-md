<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $v$ is a [cyclic vector](../../../../cyclic-vector.md) and $V\ne0$, $v\ne0$. Finite [dimension of a vector space](../../../../dimension-vector-space.md) forces a first dependence in the sequence $v,Tv,T^2v,\ldots$. Let $k\geq1$ be the smallest index with $T^kv$ in the [linear span](../../../../linear-span.md) of its predecessors. Then

$$
B=(v,Tv,\ldots,T^{k-1}v)
$$

is [linearly independent](../../../../linear-independence.md). Its [linear span](../../../../linear-span.md) $W$ is invariant under $T$: all but the last [basis](../../../../basis.md) candidate map to the next, and the last maps to $T^kv\in W$. Induction therefore puts every $T^jv$ in $W$. Cyclicity gives $W=V$, so **$B$ is a [basis](../../../../basis.md) and $k=n$**.

Write

$$
T^nv=-a_0v-a_1Tv-\cdots-a_{n-1}T^{n-1}v.
$$

The [matrix](../../../../matrix.md) of $T$ in this [basis](../../../../basis.md) is the [companion matrix](../../../../companion-matrix.md)

$$
C=\begin{pmatrix}
0&0&\cdots&0&-a_0\\
1&0&\cdots&0&-a_1\\
0&1&\cdots&0&-a_2\\
\vdots&\vdots&\ddots&\vdots&\vdots\\
0&0&\cdots&1&-a_{n-1}
\end{pmatrix}.
$$

For $p(t)=t^n+a_{n-1}t^{n-1}+\cdots+a_0$, the defining relation says $p(T)v=0$. Since $p(T)$ commutes with $T$, it also annihilates every $T^jv$ in $B$, hence $p(T)=0$. No nonzero [polynomial](../../../../polynomial-split.md) of degree less than $n$ can annihilate $v$, because that would contradict [linear independence](../../../../linear-independence.md) of $B$. Thus $m_T=p$.

Finally the [characteristic polynomial of a companion matrix](../../../../characteristic-polynomial-of-a-companion-matrix.md) is $p$, by direct [determinant](../../../../determinant.md) expansion. Explicitly, expansion along the first row of $tI-C$ gives the recurrence

$$
D_n(t;a_0,\ldots,a_{n-1})
=tD_{n-1}(t;a_1,\ldots,a_{n-1})+a_0,
$$

starting from $D_1=t+a_0$. It yields $D_n=t^n+a_{n-1}t^{n-1}+\cdots+a_0$. Consequently

$$
\boxed{m_T(t)=\chi_T(t).}
$$

This proves that a [cyclic operator has equal minimal and characteristic polynomials](../../../../cyclic-operator-has-equal-minimal-and-characteristic-polynomials.md) by the cyclic [basis](../../../../basis.md) and a direct determinant calculation, with no appeal to the [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
