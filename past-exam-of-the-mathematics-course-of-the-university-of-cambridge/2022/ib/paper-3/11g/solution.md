<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

A map $T:X\to Y$ between metric spaces is a [contraction mapping](../../../../../contraction-mapping-theorem.md) if some $q<1$ satisfies $d(Tx,Ty)\leq qd(x,y)$ for all $x,y$.

The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) states that a contraction from a nonempty complete metric space to itself has a unique fixed point. Indeed, for $x_{n+1}=Tx_n$,

$$
d(x_{n+1},x_n)\leq q^nd(x_1,x_0),
$$

so the geometric-series estimate makes $(x_n)$ Cauchy. Completeness gives a limit $x_*$, continuity gives $Tx_*=x_*$, and

$$
d(x_*,y_*)\leq qd(x_*,y_*)
$$

proves uniqueness.

Every solution of $x=\cos x$ lies in $[-1,1]$. The cosine maps this complete interval into itself and, by the [mean value theorem](../../../../../mean-value-theorem.md), has Lipschitz constant at most $\sin1<1$ there. It therefore has exactly one real fixed point.

The [mean value inequality](../../../../../mean-value-inequality.md) says that on a convex domain, a uniform derivative bound $\lVert Df\rVert\leq M$ implies $\lVert f(x)-f(y)\rVert\leq M\lVert x-y\rVert$. Equip $\mathbb R^2$ with the maximum norm and take

$$
D=[0,1/2]\times[-1/2,1/2].
$$

For $(x,y)\in D$, elementary cosine bounds give

$$
f_1(x,y)\in[\cos(1/2)-1/2,1/2],
\qquad |f_2(x,y)|\leq1-\cos(1/2)<1/2,
$$

so $f(D)\subseteq D$. The maximum absolute row sum of

$$
Df=
\begin{pmatrix}
-\tfrac12\sin x&-\tfrac12\sin y\\
-\sin x&\sin y
\end{pmatrix}
$$

is at most $2\sin(1/2)<1$. The mean value inequality makes $f$ a contraction on the complete set $D$, so it has a fixed point.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
