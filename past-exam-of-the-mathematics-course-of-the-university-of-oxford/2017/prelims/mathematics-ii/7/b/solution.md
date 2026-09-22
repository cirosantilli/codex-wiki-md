<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $E_n=\sup_{t\in[a,b]}|f(t)-\phi_n(t)|\to0$, so the hypothesis is [uniform convergence](../../../../../../uniform-convergence.md). Every [step function](../../../../../../step-function.md) is bounded and [Riemann integrable](../../../../../../riemann-integrable-function.md): away from its finitely many partition points it is constant, and those exceptional points can be covered by [intervals](../../../../../../interval-mathematics.md) of arbitrarily small total length. A [partition of an interval](../../../../../../partition-of-an-interval.md) containing their boundaries makes the difference of its [upper Darboux sum](../../../../../../upper-darboux-sum.md) and [lower Darboux sum](../../../../../../lower-darboux-sum.md) arbitrarily small.

Choose one $n$ with $E_n<\infty$. Boundedness of $\phi_n$ and $|f|\leq|\phi_n|+E_n$ show that $f$ is a [bounded function](../../../../../../bounded-function.md). Assume $a<b$, since for $a=b$ all the [integrals](../../../../../../integral-split.md) are zero. Given $\eta>0$, choose $n$ so that $2E_n(b-a)<\eta/2$, and then a [partition of an interval](../../../../../../partition-of-an-interval.md) $P$ such that $U(\phi_n,P)-L(\phi_n,P)<\eta/2$. On every partition subinterval, $|f-\phi_n|\leq E_n$ gives

$$
U(f,P)\leq U(\phi_n,P)+E_n(b-a),\qquad L(f,P)\geq L(\phi_n,P)-E_n(b-a).
$$

Thus

$$
U(f,P)-L(f,P)\leq U(\phi_n,P)-L(\phi_n,P)+2E_n(b-a)<\eta.
$$

The [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md) proves that $f$ is [Riemann integrable](../../../../../../riemann-integrable-function.md). Finally, [linearity of the integral](../../../../../../linearity-of-integration.md) and [monotonicity of the Riemann integral](../../../../../../monotonicity-of-the-riemann-integral.md) give

$$
\left|\int_a^bf(t)\,dt-\int_a^b\phi_n(t)\,dt\right|\leq\int_a^b|f(t)-\phi_n(t)|\,dt\leq(b-a)E_n\longrightarrow0.
$$

Therefore

$$
\boxed{\int_a^bf(t)\,dt=\lim_{n\to\infty}\int_a^b\phi_n(t)\,dt.}
$$

This proves the relevant case of [uniform convergence preserves integrals on a compact interval](../../../../../../uniform-convergence-preserves-integrals-on-a-compact-interval.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
