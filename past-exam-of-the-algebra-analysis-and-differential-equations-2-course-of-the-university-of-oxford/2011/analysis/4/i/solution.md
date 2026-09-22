<h1 id="analysis/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the preliminary definition, put $S_N(z)=\sum_{k=1}^Nf_k(z)$. The series converges [uniformly](../../../../../uniform-convergence.md) to $f$ on $U$ when, for every $\epsilon>0$, some $N_0$ satisfies $|S_N(z)-f(z)|<\epsilon$ for all $z\in U$ and all $N\geq N_0$. Equivalently, $\sup_{z\in U}|S_N(z)-f(z)|\to0$.

Let $L(\gamma)$ be the finite length of the piecewise-smooth path. Finite linearity of the [contour integral](../../../../../contour-integral.md) and the integral bound give

$$
\left|\sum_{k=1}^N\int_\gamma f_k(z)\,dz-\int_\gamma f(z)\,dz\right|
=\left|\int_\gamma(S_N-f)\,dz\right|
\leq L(\gamma)\sup_U|S_N-f|\longrightarrow0.
$$

The uniform limit is continuous by the stated allowed result, so its integral is defined. Consequently

$$
\boxed{\sum_{k=1}^{\infty}\int_\gamma f_k(z)\,dz=\int_\gamma f(z)\,dz.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [Analysis](../../../analysis.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
