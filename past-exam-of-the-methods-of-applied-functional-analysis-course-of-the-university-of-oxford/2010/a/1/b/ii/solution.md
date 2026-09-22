<h1 id="a/1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove existence directly through [quadratic energy minimization by the parallelogram law](../../../../../../quadratic-energy-minimization-by-the-parallelogram-law.md). Let $m=\inf_{v\in H_g^1}A[v]$. The set contains $g$, and [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) gives $0\leq m\leq A[g]<\infty$. Choose a [minimizing sequence](../../../../../../minimizing-sequence.md) $v_j$ with $A[v_j]\to m$. Since $(v_j+v_k)/2\in H_g^1$, the [parallelogram law](../../../../../../parallelogram-law.md) gives

$$
A[v_j-v_k]=2A[v_j]+2A[v_k]-4A[(v_j+v_k)/2]\leq2A[v_j]+2A[v_k]-4m\longrightarrow0.
$$

The differences belong to $H_0^1$, so [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) and the [Poincaré inequality](../../../../../../poincare-inequality.md) imply

$$
\|v_j-v_k\|_{H^1}^2\leq\frac{1+C_P^2}{\lambda}A[v_j-v_k]\longrightarrow0.
$$

Thus $(v_j)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). Completeness of $H_0^1$, applied to $v_j-g$, produces $u\in H_g^1$ with $v_j\to u$ in $H^1$. The bounded coefficient matrix makes $a$ a [bounded bilinear form](../../../../../../bounded-bilinear-form.md), so $A[v_j]\to A[u]$. Consequently $A[u]=m$, and part (i) makes $u$ a [weak solution](../../../../../../weak-solution.md).

For uniqueness, the difference $w$ of two [weak solutions](../../../../../../weak-solution.md) lies in $H_0^1$ and satisfies $a(w,w)=0$. [Uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) gives $\nabla w=0$ almost everywhere, and the [Poincaré inequality](../../../../../../poincare-inequality.md) gives $w=0$. The argument proves existence and uniqueness without assuming the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
