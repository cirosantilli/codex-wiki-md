<h1 id="algebra/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

If $c(\lambda)=\det(\lambda I-T)=0$, then $\lambda I-T$ has nonzero [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md). A nonzero vector $v$ in that [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md) satisfies $Tv=\lambda v$, proving that $\lambda$ is an [eigenvalue](../../../../eigenvalue.md). Extend $v$ to a [basis](../../../../basis.md). Its first column is $(\lambda,0,\ldots,0)^T$, so the [matrix](../../../../matrix.md) has block form

$$
[T]=\begin{pmatrix}\lambda&*\\0&B\end{pmatrix},\qquad c(X)=(X-\lambda)\det(XI-B).
$$

Here $B$ represents the induced operator on $V/\langle v\rangle$.

If the [algebraic multiplicity](../../../../algebraic-multiplicity.md) is $r$, repeat this argument in that quotient: its [characteristic polynomial](../../../../characteristic-polynomial.md) still has $\lambda$ with multiplicity $r-1$. Induction and lifting a quotient [basis](../../../../basis.md) gives a [basis](../../../../basis.md) whose first $r$ columns have the prescribed upper-triangular form. With $U$ the span of those $r$ vectors, the full [matrix](../../../../matrix.md) is

$$
\begin{pmatrix}\lambda I+N&*\\0&C\end{pmatrix},\qquad N^r=0,\qquad\det(C-\lambda I)\ne0.
$$

Thus $U$ is invariant and is contained in $W_\lambda$. Conversely, if $(T-\lambda I)^sv=0$, project to $V/U$. The induced map $C-\lambda I$ is invertible, so its $s$th power cannot kill a nonzero class. Hence $v\in U$. Consequently $\boxed{W_\lambda=U,\ \dim W_\lambda=r}$; this proves simultaneously that it is a [subspace](../../../../vector-subspace.md) and $T$-invariant. It also proves $(T-\lambda I)^r=0$ on this space, without using [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md) in advance.

To prove independence of the different spaces, take a relation $\sum_\lambda v_\lambda=0$ with $v_\lambda\in W_\lambda$. Fix $\lambda$ and apply $P_\lambda(T)=\prod_{\mu\ne\lambda}(T-\mu I)^{r_\mu}$. It kills all terms except $v_\lambda$. On $W_\lambda$, each factor $T-\mu I=(\lambda-\mu)I+N$ is invertible: its inverse is a finite [geometric series](../../../../geometric-series.md) in the [nilpotent](../../../../nilpotent-linear-map.md) $N$. Hence $P_\lambda(T)v_\lambda=0$ implies $v_\lambda=0$. The sum is direct, and its [dimension](../../../../dimension-vector-space.md) is $\sum r_\lambda=\dim V$, so

$$
\boxed{V=\bigoplus_\lambda W_\lambda.}
$$

Finally $c(T)=\prod_\lambda(T-\lambda I)^{r_\lambda}$ kills each summand, hence every vector. This proves $\boxed{c(T)=0}$ without circularly assuming the theorem during the decomposition.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Algebra](../../algebra.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
