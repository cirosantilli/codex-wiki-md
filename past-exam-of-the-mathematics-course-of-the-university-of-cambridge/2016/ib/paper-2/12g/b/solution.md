<h1 id="12g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [linear map](../../../../../../linear-map.md) $A:\mathbb R^m\to\mathbb R^n$, define the [operator norm](../../../../../../operator-norm.md) by

$$
\boxed{\|A\|=\sup_{x\ne0}\frac{\|Ax\|}{\|x\|}=\sup_{\|x\|=1}\|Ax\|.}
$$

It is finite. To see this without assuming continuity of $A$, write $x=\sum x_j e_j$: the [triangle inequality](../../../../../../triangle-inequality.md) bounds $\|Ax\|$ by $\sum|x_j|\|Ae_j\|$. Every [norm](../../../../../../norm.md) in finite dimensions is equivalent to the [Euclidean norm](../../../../../../euclidean-norm.md). One proof first uses this same coordinate bound to establish continuity of the [norm](../../../../../../norm.md) on the Euclidean unit sphere; [compactness](../../../../../../compact-space.md) then gives a strictly positive minimum there. Thus the coordinate bound above is at most a fixed multiple of $\|x\|$.

Absolute homogeneity and the [triangle inequality](../../../../../../triangle-inequality.md) for this [operator norm](../../../../../../operator-norm.md) follow from those for $\|Ax\|$ and taking suprema. If $\|A\|=0$, then $Ax=0$ for every $x$, hence $A=0$, and the converse is immediate. For any $B:\mathbb R^\ell\to\mathbb R^m$, the defining bound $\|Ax\|\le\|A\|\|x\|$ gives

$$
\|ABx\|\le\|A\|\|Bx\|\le\|A\|\|B\|\|x\|,
\qquad \boxed{\|AB\|\le\|A\|\|B\|.}
$$

This is [submultiplicativity of the operator norm](../../../../../../submultiplicativity-of-the-operator-norm.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12G](../../12g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
