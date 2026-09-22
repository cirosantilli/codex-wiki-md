<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The convergence is in the [strong operator topology](../../../../strong-operator-topology.md): for each fixed $f\in E$, one must prove $\|\lambda R_\lambda f-f\|\to0$. First, the [contraction semigroup](../../../../contraction-semigroup.md) bound gives

$$
\|\lambda R_\lambda f\|
\leq\int_0^\infty\lambda e^{-\lambda t}\|P_tf\|\,dt
\leq\|f\|.
$$

Thus **$\lambda R_\lambda$ is a contraction**. This is the useful scaling of the contraction estimate in the source's hint. Since $\int_0^\infty\lambda e^{-\lambda t}\,dt=1$,

$$
\lambda R_\lambda f-f
=\int_0^\infty\lambda e^{-\lambda t}(P_tf-f)\,dt.
$$

Fix $\varepsilon>0$. By [strong continuity](../../../../strong-continuity.md), choose $\delta>0$ so that $\|P_tf-f\|<\varepsilon$ for $0\leq t\leq\delta$. Split the integral there and use $\|P_tf-f\|\leq2\|f\|$ for the tail:

$$
\begin{aligned}
\|\lambda R_\lambda f-f\|
&\leq\varepsilon\int_0^\delta\lambda e^{-\lambda t}\,dt
+2\|f\|\int_\delta^\infty\lambda e^{-\lambda t}\,dt\\
&\leq\varepsilon+2\|f\|e^{-\lambda\delta}.
\end{aligned}
$$

Let $\lambda\to\infty$ and then $\varepsilon\downarrow0$. Therefore

$$
\boxed{\lambda R_\lambda f\longrightarrow f\text{ in }E\quad\text{for every }f\in E.}
$$

The distinction from [operator norm](../../../../operator-norm.md) convergence is essential. For example, the [multiplication semigroup](../../../../multiplication-semigroup.md) on $\ell^2(\mathbb N)$ defined by $(P_tf)_n=e^{-nt}f_n$ is a [strongly continuous semigroup](../../../../c0-semigroup.md) of contractions: coordinatewise convergence and [dominated convergence](../../../../dominated-convergence-theorem.md) applied to $\sum_n|f_n|^2$ prove [strong continuity](../../../../strong-continuity.md). Its [resolvent operator](../../../../resolvent-of-an-operator.md) is $(R_\lambda f)_n=f_n/(\lambda+n)$, and

$$
\|\lambda R_\lambda-I\|=\sup_{n\geq1}\frac n{\lambda+n}=1.
$$

Thus the claimed convergence cannot in general be read as convergence in [operator norm](../../../../operator-norm.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
