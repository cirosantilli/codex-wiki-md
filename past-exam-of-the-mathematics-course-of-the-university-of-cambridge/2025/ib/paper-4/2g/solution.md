<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

A contraction satisfies $d(Tx,Ty)\le qd(x,y)$ for some $0\le q<1$. Starting from $x_0$, define $x_{k+1}=Tx_k$. The geometric bound on successive distances makes $(x_k)$ Cauchy, so completeness gives a [limit](../../../../../limit-of-a-function.md) $x$. Continuity of $T$ gives $Tx=x$. If $Ty=y$, then $d(x,y)\le qd(x,y)$, hence $x=y$. This is the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md).

If $T^n$ is a contraction, it has a unique fixed point $x$. Since $T^n(Tx)=T(T^nx)=Tx$, the point $Tx$ is also fixed by $T^n$, so uniqueness gives $Tx=x$. Every fixed point of $T$ is fixed by $T^n$, so it too must equal $x$. Thus $T$ has exactly one fixed point.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
