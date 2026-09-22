<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

In the usual nondegenerate convention, a [strongly regular graph](../../../../../strongly-regular-graph.md) of order $n$ and parameters $(d,a,b)$ is a finite simple $d$-regular graph with $0<d<n-1$ in which adjacent vertices have $a$ common neighbours and distinct nonadjacent vertices have $b$. Its [adjacency matrix of a graph](../../../../../adjacency-matrix.md) $A$ obeys

$$
A^2=(d-b)I+(a-b)A+bJ.
$$

For the usual nondegenerate parameters with $b>0$ the graph is connected, so [eigenvalue](../../../../../eigenvalue.md) $d$ has multiplicity one. On the perpendicular complement of the all-ones vector, $J=0$ and the possible [eigenvalues](../../../../../eigenvalue.md) are

$$
r,s=\frac{a-b\pm\Delta}{2},\qquad
\Delta=\sqrt{(a-b)^2+4(d-b)}.
$$

If $r$ has multiplicity $m$, then zero [trace](../../../../../matrix-trace.md) gives $d+mr+(n-1-m)s=0$. Solving proves

$$
\boxed{m=\frac12\left[n-1+\frac{(n-1)(b-a)-2d}{\Delta}\right]\in\mathbb Z}.
$$

The denominator is positive in this nondegenerate convention. Otherwise all [eigenvalues](../../../../../eigenvalue.md) on the all-ones complement would coincide, forcing $A=rI+(d-r)J/n$. All off-diagonal entries would then be the same, making the graph complete or edgeless. If complete graphs are admitted with arbitrary unused $b$, the printed claim needs qualification: $K_2$ with $(d,a,b)=(1,0,2)$ satisfies the common-neighbour conditions vacuously but makes the fraction $0/0$. For complete graphs with nonzero denominator, the spectral calculation still works with an unused root of multiplicity zero.

For the [triangle-free graph](../../../../../triangle-free-graph.md) claim, suppose first there are at least two vertices. Nonadjacent vertices have a common neighbour, so the graph is connected. If $u,v$ are adjacent, put $U=N(u)\setminus\{v\}$ and $V=N(v)\setminus\{u\}$. Every member of $U$ is nonadjacent to $v$, and exactly two of its three common neighbours with $v$ lie in $V$, the third being $u$. By symmetry every member of $V$ has exactly two neighbours in $U$. Counting these edges gives $2|U|=2|V|$, hence $d(u)=d(v)$. Connectivity makes the graph $d$-regular. Counting length-two paths from a vertex to non-neighbours gives

$$
3(n-d-1)=d(d-1),\qquad \boxed{n=1+d(d+2)/3}.
$$

Here $a=0$, $b=3$, and the larger-root multiplicity becomes $[n-1+d^2/\sqrt{4d-3}]/2$. Thus $t=\sqrt{4d-3}$ is rational and therefore an integer. It is odd, $d=(t^2+3)/4$, and integrality also gives $t\mid d^2$. Since $16d^2\equiv9\pmod t$, one obtains $t\mid9$, hence

$$
\boxed{t\in\{1,3,9\},\qquad d\in\{1,3,21\}}.
$$

The [complete bipartite graph](../../../../../complete-bipartite-graph.md) $K_{3,3}$ realizes $d=3$: vertices in the same part have all three vertices of the other part as common neighbours, and vertices in opposite parts are adjacent. There are no triangles.

As literally worded, the one-vertex graph is a vacuous exception: it has no triangles or nonadjacent distinct pairs, but has $d=0$. The displayed positive-degree classification therefore requires at least two vertices. This qualification completes the [triangle-free graphs with three common neighbours](../../../../../triangle-free-graphs-with-three-common-neighbours.md) argument rather than silently excluding a counterexample.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
