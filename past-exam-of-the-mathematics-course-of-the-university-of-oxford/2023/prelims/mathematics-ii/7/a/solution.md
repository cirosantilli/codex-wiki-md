<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume, as required for the displayed integrals, that the $f_n$ are [Riemann integrable](../../../../../../riemann-integrable-function.md) on $[a,b]$. Their [uniform limit](../../../../../../uniform-limit.md) $f$ is also [Riemann integrable](../../../../../../riemann-integrable-function.md): if $\sup|f-f_N|<\varepsilon$, the upper and lower [Darboux sums](../../../../../../darboux-sum.md) for a [partition of an interval](../../../../../../partition-of-an-interval.md) differ for $f$ by at most the corresponding difference for $f_N$ plus $2\varepsilon(b-a)$. Choosing $N$ and then a sufficiently fine [partition of an interval](../../../../../../partition-of-an-interval.md) proves the [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md) for $f$.

The integral estimate then gives

$$
\left|\int_a^b f_n(x)\,dx-\int_a^b f(x)\,dx\right|
\leq(b-a)\sup_{x\in[a,b]}|f_n(x)-f(x)|\longrightarrow0.
$$

This proves that [uniform convergence preserves integrals on a compact interval](../../../../../../uniform-convergence-preserves-integrals-on-a-compact-interval.md). Some integrability hypothesis is necessary: [uniform convergence](../../../../../../uniform-convergence.md) alone cannot make the integral of an arbitrary starting [function](../../../../../../function-split.md) exist.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
