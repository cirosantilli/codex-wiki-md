<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Runge-Kutta method](../../../../../../runge-kutta-method.md) has update $y_{n+1}=y_n+h\sum_i b_i k_i$. Expanding its squared [Euclidean norm](../../../../../../euclidean-norm.md) gives the exact identity

$$
\lVert y_{n+1}\rVert^2-\lVert y_n\rVert^2=h\left[2\sum_i b_i y_n^Tk_i+h\left\lVert\sum_i b_i k_i\right\rVert^2\right].
$$

The stated per-step relation makes this difference zero. Induction from the initial vector then proves

$$
\boxed{\lVert y_n\rVert=\lVert y_0\rVert\quad\text{for all computed steps}.}
$$

For a positive step size the relation is also necessary for exact per-step norm conservation. This algebraic identity applies whenever the stage equations define a step; it does not silently assume solvability of arbitrary implicit stages.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
