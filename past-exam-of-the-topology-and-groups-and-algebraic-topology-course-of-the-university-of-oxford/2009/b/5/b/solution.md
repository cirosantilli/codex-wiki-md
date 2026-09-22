<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The identifications yield one vertex, $g$ one-cells and one two-cell, whose boundary word is $a_1^2\cdots a_g^2$. Thus the integral [cellular chain complex](../../../../../cellular-chain-complex.md), in degrees two, one and zero, has

$$
C_2=\mathbb Z,\quad C_1=\mathbb Z^g,\quad C_0=\mathbb Z,\qquad
\partial_2(1)=(2,\ldots,2),\quad\partial_1=0.
$$

For $g\geq1$ the first map is injective. The vector $(1,\ldots,1)$ is primitive and extends to an integral basis, so quotienting by twice that vector gives

$$
\boxed{H_k(N_g;\mathbb Z)=\begin{cases}
\mathbb Z,&k=0,\\
\mathbb Z^{g-1}\oplus\mathbb Z/2,&k=1,\\
0,&k\geq2.
\end{cases}}
$$

With $\mathbb F_2=\mathbb Z/2\mathbb Z$, every boundary map vanishes. Hence

$$
\boxed{H_k(N_g;\mathbb F_2)=\begin{cases}
\mathbb F_2,&k=0,2,\\
\mathbb F_2^g,&k=1,\\
0,&k>2.
\end{cases}}
$$

For [cohomology](../../../../../cohomology-split.md), dualize the free cellular complex. The only nonzero possible coboundary over $\mathbb Z$ is $\delta^1:\mathbb Z^g\to\mathbb Z$, $(v_1,\ldots,v_g)\mapsto2\sum_i v_i$. Its kernel is free of rank $g-1$ and its image is $2\mathbb Z$. Thus

$$
\boxed{H^k(N_g;\mathbb Z)=\begin{cases}
\mathbb Z,&k=0,\\
\mathbb Z^{g-1},&k=1,\\
\mathbb Z/2,&k=2,\\
0,&k>2.
\end{cases}}
$$

Over $\mathbb F_2$ the cochain maps are zero too, giving $H^0=H^2=\mathbb F_2$, $H^1=\mathbb F_2^g$, and zero higher groups. In particular the integral top homology and top [cohomology](../../../../../cohomology-split.md) differ, as their explicit complexes show. Finally the cell count gives

$$
\boxed{\chi(N_g)=1-g+1=2-g}.
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
