<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

We prove [uniform continuity](../../../../../uniform-continuity.md) by contradiction. If it fails, there is $\varepsilon_0>0$ such that, for every $n\geq1$, we can choose $x_n,y_n\in X$ with

$$
d(x_n,y_n)<1/n,\qquad \rho(f(x_n),f(y_n))\geq\varepsilon_0.
$$

By [sequential compactness](../../../../../sequentially-compact-space.md), pass to a [subsequence](../../../../../subsequence.md) with $x_{n_k}\to x\in X$. The [triangle inequality](../../../../../triangle-inequality.md) gives

$$
d(y_{n_k},x)\leq d(y_{n_k},x_{n_k})+d(x_{n_k},x)\longrightarrow0.
$$

By [continuity](../../../../../continuous-function.md), both $f(x_{n_k})$ and $f(y_{n_k})$ converge to $f(x)$. A second [triangle inequality](../../../../../triangle-inequality.md) therefore gives

$$
\rho(f(x_{n_k}),f(y_{n_k}))\leq\rho(f(x_{n_k}),f(x))+\rho(f(x),f(y_{n_k}))\longrightarrow0,
$$

contradicting the lower bound. Thus the requested $\delta$, independent of $x,y$, exists for every $\varepsilon>0$.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
