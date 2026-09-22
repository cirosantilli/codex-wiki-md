<h1 id="14i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Count edges from the $k$ neighbours of a fixed vertex to its $n-k-1$ nonneighbours. Each neighbour contributes $k-a-1$ such edges, and each nonneighbour receives $b$. With $a=0,b=3$,

$$
3(n-k-1)=k(k-1),\qquad n=\frac{k^2+2k+3}{3}.
$$

The graph is incomplete, so there are nonadjacent vertices and $k\geq3$. Substituting into the [eigenvalue multiplicity](../../../../../../eigenvalue-multiplicity.md) formula gives a multiplicity difference of $k^2/\sqrt{4k-3}$. This must be an integer. As $k>0$, $d=\sqrt{4k-3}$ is rational and hence an integer; it is positive and odd. Moreover $d\mid k^2$ and $4k=d^2+3$, so reducing $16k^2$ modulo $d$ gives $d\mid9$. Thus $d\in\{1,3,9\}$. The value $d=1$ gives $k=1$, impossible here; the other two give $(k,n)=(3,6)$ and $(21,162)$. Consequently **$|G|\in\{6,162\}$**. This is a necessity argument, not a claim that integrality alone constructs either graph.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14I](../../14i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
