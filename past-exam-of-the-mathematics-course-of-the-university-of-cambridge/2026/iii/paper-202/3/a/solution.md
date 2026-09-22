<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the level-$N$ dyadic partition, write

$$
V_N(t)=\sum_{k=1}^{2^N}
|f(k2^{-N}\wedge t)-f((k-1)2^{-N}\wedge t)|.
$$

The dyadic partitions are nested, so the [triangle inequality](../../../../../../triangle-inequality.md) makes $V_N(t)$ nondecreasing in $N$, and $\lVert f_t\rVert=\lim_NV_N(t)$.

Fix $t_1<t_2$. As the mesh tends to zero, the last dyadic point before $t_1$ approaches $t_1$. Refining from there to $t_2$, the triangle inequality says that the added variation is at least $|f(t_2)-f(t_1)|$ minus the two endpoint errors, which tend to zero by [continuity](../../../../../../continuous-function.md). Therefore

$$
\lim_N\bigl(V_N(t_2)-V_N(t_1)\bigr)
\geq|f(t_2)-f(t_1)|.
$$

Since $\lVert f\rVert<\infty$, both limits are finite and may be subtracted, giving

$$
\boxed{\lVert f_{t_2}\rVert-\lVert f_{t_1}\rVert
\geq|f(t_2)-f(t_1)|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
