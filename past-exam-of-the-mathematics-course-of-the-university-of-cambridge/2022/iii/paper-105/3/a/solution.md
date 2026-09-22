<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $B$ and $F$ satisfy the hypotheses of the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md). By the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md), there are a bounded linear operator $T:H\to H$ and $z\in H$ such that

$$
B(u,v)=(Tu,v)_H,
\qquad
F(v)=(z,v)_H.
$$

Coercivity and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply

$$
\alpha\lVert u\rVert_H^2\leq(Tu,u)_H
\leq\lVert Tu\rVert_H\lVert u\rVert_H,
$$

so $\lVert Tu\rVert_H\geq\alpha\lVert u\rVert_H$. Thus $T$ is injective and its range is closed. If $y$ is orthogonal to its range, then $B(x,y)=0$ for every $x$; taking $x=y$ and using coercivity gives $y=0$. The range is therefore dense as well as closed, hence all of $H$. There is a unique $u=T^{-1}z$, and it satisfies $B(u,v)=F(v)$ for all $v$. The lower bound also gives $\lVert u\rVert_H\leq\lVert F\rVert/\alpha$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
