<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The printed assertion needs an endpoint qualification:** the enumeration includes zero, but $\mathbf1_{[0,0)}$ is identically zero. In fact $f$ is continuous at zero; the claimed [discontinuities](../../../../../../discontinuity.md) occur at every $r_j>0$.

Define the finite [step function](../../../../../../step-function.md) sums

$$
\phi_N(t)=\sum_{k=1}^N\frac1{k^2}\mathbf1_{[0,r_k)}(t).
$$

The assumed convergence of $\sum_k1/k^2$ and the bound on each [indicator function](../../../../../../indicator-function.md) give

$$
0\leq f(t)-\phi_N(t)\leq\sum_{k>N}\frac1{k^2},\qquad\|f-\phi_N\|_\infty\leq\sum_{k>N}\frac1{k^2}\longrightarrow0.
$$

Thus the defining [series](../../../../../../series-mathematics.md) converges everywhere and has [uniform convergence](../../../../../../uniform-convergence.md). Part (b) proves that **$f$ is [Riemann integrable](../../../../../../riemann-integrable-function.md)**; it also gives, if desired,

$$
\boxed{\int_0^1f(t)\,dt=\sum_{k=1}^{\infty}\frac{r_k}{k^2}.}
$$

For $r_j>0$ and $0\leq t<r_j$, every [indicator function](../../../../../../indicator-function.md) is [nonincreasing](../../../../../../nonincreasing-function.md), and the $j$th drops by one between $t$ and $r_j$. Hence

$$
f(t)-f(r_j)=\sum_{k\geq1}\frac{\mathbf1_{[0,r_k)}(t)-\mathbf1_{[0,r_k)}(r_j)}{k^2}\geq\frac1{j^2}.
$$

Taking inputs from the left tending to $r_j$ proves a [discontinuity](../../../../../../discontinuity.md) there.

For completeness, [continuity](../../../../../../continuous-function.md) at zero follows directly from a finite-head and tail argument. Given $\varepsilon>0$, choose $N$ with $\sum_{k>N}1/k^2<\varepsilon$. Choose $\delta>0$ below every positive $r_k$ with $k\leq N$. For $0\leq t<\delta$, the first $N$ [indicator functions](../../../../../../indicator-function.md) have exactly their values at zero; the one with $r_k=0$, if present, is always zero. Thus $|f(t)-f(0)|\leq\sum_{k>N}1/k^2<\varepsilon$. This confirms that the endpoint exception is real. Replacing the printed enumeration of $[0,1)$ by one of $(0,1)$ would remove it.

Finally, the [density of the rational numbers](../../../../../../density-of-the-rational-numbers.md) supplies a positive rational $r_j$ in every nonempty open subinterval of $[0,1]$. Thus **a [Riemann integrable](../../../../../../riemann-integrable-function.md) [function](../../../../../../function-split.md) can have a [discontinuity](../../../../../../discontinuity.md) in every open subinterval**: [dense jumps do not prevent Riemann integrability](../../../../../../dense-jumps-do-not-prevent-riemann-integrability.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
