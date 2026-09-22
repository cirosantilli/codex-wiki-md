<h1 id="11f/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The appropriate [homotopy invariance of winding number](../../../../../../homotopy-invariance-of-winding-number.md) is: if $H:[0,1]^2\to\mathbb C\setminus\{0\}$ is continuous and $H(s,0)=H(s,1)$ for each $s$, then all loops $t\mapsto H(s,t)$ have the same [winding number](../../../../../../winding-number.md). The basepoint may move; every intermediate curve must close and avoid zero.

[Compactness](../../../../../../compact-space.md) gives $m=\min_{s,t}|H(s,t)|>0$. [Uniform continuity](../../../../../../uniform-continuity.md) gives $\delta>0$ such that $|s-s'|<\delta$ implies $|H(s,t)-H(s',t)|<m$ for every $t$. Part (d) then makes the [winding numbers](../../../../../../winding-number.md) equal for nearby $s,s'$. Subdivide $[0,1]$ into steps smaller than $\delta$ and chain these equalities. Therefore

$$
\boxed{w(H(0,\cdot))=w(H(1,\cdot)).}
$$

This proves the theorem directly for continuous loops, without requiring an integral formula or smooth [homotopy](../../../../../../homotopy.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [11F](../../11f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
