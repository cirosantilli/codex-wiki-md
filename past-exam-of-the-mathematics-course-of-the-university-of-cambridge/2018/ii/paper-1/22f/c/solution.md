<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $C(K)$ is [equicontinuous](../../../../../../equicontinuity.md). At each $x\in K$, choose a neighbourhood $U$ such that

$$
|f(y)-f(x)|<1
$$

for every $y\in U$ and every $f\in C(K)$. If some $y\in U$ differed from $x$, the [Urysohn lemma](../../../../../../urysohn-s-lemma.md) for the compact Hausdorff space $K$ would give a continuous function with $f(x)=0$ and $f(y)=2$, a contradiction. Thus every singleton is open, so $K$ is discrete. A compact discrete space is finite, proving

$$
\boxed{\ C(K)\text{ equicontinuous}\Longrightarrow K\text{ finite}.\ }
$$

Compactness is essential. Any infinite set with the discrete topology has equicontinuous $C(K)$, because the singleton neighbourhood $\{x\}$ works simultaneously for every function, but the space is infinite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
