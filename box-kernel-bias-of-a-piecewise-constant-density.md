# Box-kernel bias of a piecewise constant density

↑ **Parent:** [Integrated squared bias from a density jump](integrated-squared-bias-from-a-density-jump.md)

For a density with finitely many jumps $\Delta_r$ at separated points and the [unit-width box kernel](unit-width-box-kernel.md), take $h$ smaller than all consecutive jump spacings. The smoothing bias is supported in disjoint length-$h$ neighbourhoods of the jumps. At each jump its two sides form triangles of height $|\Delta_r|/2$, and exact integration gives

$$
\|K_h*f-f\|_2^2=\frac h{12}\sum_r\Delta_r^2.
$$

Combined with the [integrated variance of a kernel density estimator](integrated-variance-of-a-kernel-density-estimator.md), this gives expected $L^2$ error $O(n^{-1/4})$ at $h\asymp n^{-1/2}$.

## ↑ Ancestors (11)

1. [Integrated squared bias from a density jump](integrated-squared-bias-from-a-density-jump.md)
2. [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)
3. [Kernel density estimation](kernel-density-estimation.md)
4. [Kernel for density estimation](kernel-for-density-estimation.md)
5. [Density estimation](density-estimation.md)
6. [Nonparametric statistics](nonparametric-statistics-split.md)
7. [Statistical inference](statistical-inference-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/2/solution.md)
