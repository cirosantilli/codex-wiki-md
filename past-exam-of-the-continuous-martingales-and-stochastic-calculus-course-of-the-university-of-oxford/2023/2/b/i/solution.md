<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

To establish the [Brownian weighted quadratic variation in L2](../../../../../brownian-weighted-quadratic-variation-in-l2.md) for the deterministic [partition of an interval](../../../../../partition-of-an-interval.md), decompose

$$
\sum_jB_j(\Delta B_j)^2-\int_0^tB_s\,ds
=U_\pi+V_\pi,
$$

where $U_\pi=\sum_jB_j((\Delta B_j)^2-\Delta t_j)$ and $V_\pi=\sum_jB_j\Delta t_j-\int_0^tB_sds$.

The summands in $U_\pi$ are [martingale differences](../../../../../martingale-difference.md): $B_j$ is $\mathcal F_{t_j}$-[measurable](../../../../../measurability.md), and the following [Brownian increment](../../../../../brownian-increment.md) is [independent](../../../../../independent-random-variables.md) of $\mathcal F_{t_j}$. Their conditional [means](../../../../../expected-value-split.md) are zero, so distinct summands are [orthogonal](../../../../../orthogonal-vectors.md) in [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Since $\mathbb EB_j^2=t_j$ and $\mathbb E[((\Delta B_j)^2-\Delta t_j)^2]=2(\Delta t_j)^2$,

$$
\mathbb EU_\pi^2=2\sum_jt_j(\Delta t_j)^2
\leq2t^2|\pi|\longrightarrow0.
$$

For the [Riemann sum](../../../../../riemann-sum.md) error, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\mathbb EV_\pi^2
\leq t\sum_j\int_{t_j}^{t_{j+1}}\mathbb E|B_j-B_s|^2ds
=\frac t2\sum_j(\Delta t_j)^2
\leq\frac{t^2|\pi|}{2}\longrightarrow0.
$$

Thus the triangle inequality in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) proves

$$
\boxed{\sum_jB_j(\Delta B_j)^2
\longrightarrow\int_0^tB_s\,ds\quad\text{in }L^2(\mathbb P).}
$$

The time integration variable is $s$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
