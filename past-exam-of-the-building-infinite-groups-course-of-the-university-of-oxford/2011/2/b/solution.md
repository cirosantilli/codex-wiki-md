<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose finite symmetric generating sets $S_i$ for all $G_i$, and let $L\ge1$ bound the $S$-length of their elements. If $[G_{i-1}:G_i]=\infty$, the connected locally finite [Schreier graph](../../../../schreier-graph.md) of left cosets of $G_i$ in $G_{i-1}$ is infinite. Its radius-$r$ [ball](../../../../ball-mathematics.md) has at least $r+1$ vertices: otherwise a finite-diameter locally finite connected graph would be finite. Equivalently, we can choose $r+1$ distinct left-[coset](../../../../coset.md) representatives $t_{i,0},\ldots,t_{i,r}$ of $G_i$, each of $S_{i-1}$-length at most $r$, and hence $S$-length at most $Lr$.

The $(r+1)^n$ products

$$
t_{1,j_1}t_{2,j_2}\cdots t_{n,j_n}\qquad(0\le j_i\le r)
$$

are distinct. Indeed, equality first forces equality of the $G_1$-cosets of the first factors, and hence their indices; cancellation then forces equality of the $G_2$-cosets of the second factors, and so on. Each product has $S$-length at most $nLr$. Therefore

$$
(r+1)^n\le|B_S(nLr)|\le C(1+nLr)^d.
$$

Letting $r\to\infty$ yields

$$
\boxed{n\le d.}
$$

For $n=0$ the assertion is automatic.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the building infinite groups course of the University of Oxford](../../../split.md)
5. [Building infinite groups course of the University of Oxford](../../../../building-infinite-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
