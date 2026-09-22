<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

A [compact space](../../../../../compact-space.md) is one for which every open cover has a finite subcover. Let $\mathcal U$ cover $[0,1]$, and let

$$
A=\{x\in[0,1]:[0,x]\text{ has a finite subcover from }\mathcal U\}.
$$

The set is nonempty. If $s=\sup A<1$, choose $U\in\mathcal U$ containing $s$. An interval about $s$ lies in $U$; a point of $A$ just to the left of $s$ then extends the finite cover beyond $s$, contradicting the definition of the supremum. Hence $s=1$, and the same neighbourhood argument covers $1$, proving $[0,1]$ compact.

The continuous map $t\mapsto(\cos2\pi t,\sin2\pi t)$ maps $[0,1]$ onto $S^1$. A continuous image of a compact space is compact: pull an open cover back, choose a finite subcover, and push the corresponding sets forward. Thus $S^1$ is compact.

In the unusual topology on $X=\mathbb R^2\setminus\{0\}$, a proper closed set is a finite union of punctured lines through the origin. Take any nonempty member $U$ of an open cover. Its complement is such a finite union. Each punctured line has the indiscrete subspace topology, because every other vector subspace meets it only at the removed origin, and is therefore compact. Finitely many finite subcovers, together with $U$, cover $X$. Hence **$X$ is compact**.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
