<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The sequence has [uniform convergence](../../../../../uniform-convergence.md) to $f$ when, for every $\varepsilon>0$, there is an $N$ independent of $x$ such that $|f_n(x)-f(x)|<\varepsilon$ for every $n\ge N$ and every $x\in[a,b]$. Fix $x$ and choose a single $N$ with $\|f_N-f\|_\infty<\varepsilon/3$. By [continuity](../../../../../continuous-function.md) of $f_N$, sufficiently small $|y-x|$ within the interval gives $|f_N(y)-f_N(x)|<\varepsilon/3$. The [triangle inequality](../../../../../triangle-inequality.md) then gives

$$
|f(y)-f(x)|\le|f(y)-f_N(y)|+|f_N(y)-f_N(x)|+|f_N(x)-f(x)|<\varepsilon.
$$

This proves [continuity](../../../../../continuous-function.md) at every point, including endpoints with the relative topology.

For the moving points, use the just-proved [continuity](../../../../../continuous-function.md) of $f$:

$$
\boxed{|f_n(x_n)-f(x)|\le\|f_n-f\|_\infty+|f(x_n)-f(x)|\longrightarrow0.}
$$

This is [uniform convergence at moving evaluation points](../../../../../uniform-convergence-at-moving-evaluation-points.md): uniform control is what allows the evaluation point to vary with $n$.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
