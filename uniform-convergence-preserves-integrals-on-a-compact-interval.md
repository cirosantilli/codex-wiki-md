# Uniform convergence preserves integrals on a compact interval

↑ **Parent:** [Uniform convergence](uniform-convergence.md)

If [Riemann integrable](riemann-integrable-function.md) [functions](function-split.md) $f_n:[a,b]\to\mathbb R$ converge by [uniform convergence](uniform-convergence.md) to $f$, then $f$ is [Riemann integrable](riemann-integrable-function.md) and

$$
\left|\int_a^b f_n(x)\,dx-\int_a^b f(x)\,dx\right|\leq(b-a)\|f_n-f\|_\infty\longrightarrow0.
$$

This concerns one fixed [compact interval](compact-interval.md), with finite length.[Basic Analysis: Introduction to Real Analysis, Volume I by Jiří Lebl, §6.2.2, Theorem 6.2.4](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/6-2-interchange-of-limits.md)

Here is a proof outline that also establishes [Riemann integrability](riemann-integrable-function.md) of the [uniform limit](uniform-limit.md). Assume $a<b$, and put $\ell=b-a$ and $E_N=\|f_N-f\|_\infty$. One bounded $f_N$ and finite $E_N$ show that $f$ is a [bounded function](bounded-function.md). For any [partition of an interval](partition-of-an-interval.md) $P$, its [upper Darboux sum](upper-darboux-sum.md) and [lower Darboux sum](lower-darboux-sum.md) satisfy

$$
U(f,P)-L(f,P)\leq U(f_N,P)-L(f_N,P)+2\ell E_N.
$$

Given $\eta>0$, choose $N$ with $E_N<\eta/(4\ell)$, then a [partition of an interval](partition-of-an-interval.md) with $U(f_N,P)-L(f_N,P)<\eta/2$. The displayed gap is below $\eta$, proving [Riemann integrability](riemann-integrable-function.md). Finally, $|f_n-f|\leq E_n$ and [monotonicity of the Riemann integral](monotonicity-of-the-riemann-integral.md) give the stated error estimate. When $a=b$, every [integral](integral-split.md) is zero.

For the [polynomial functions](polynomial-function.md) $f_n(x)=x^n$ on $[0,0.8]$, direct [integration](integral-split.md) and the uniform bound give

$$
\int_0^{0.8}x^n\,dx=\frac{0.8^{n+1}}{n+1}\leq0.8\cdot0.8^n\longrightarrow0.
$$

At $n=21$, the exact [integral](integral-split.md) is approximately $0.0003353953$, while the general error bound is approximately $0.0073786976$. The bound certifies the result without an exact [antiderivative](antiderivative.md). On $[0,1]$, these same [integrals](integral-split.md) still tend to zero, although there is no [uniform convergence](uniform-convergence.md): sufficient conditions need not be necessary. On an unbounded [interval](interval-mathematics.md), even [uniform convergence](uniform-convergence.md) can fail to control total area, as [uniformly vanishing functions can retain a nonzero integral](uniformly-vanishing-functions-can-retain-a-nonzero-integral.md) shows.

[Uniform convergence](uniform-convergence.md) alone also fails to preserve [derivatives](derivative.md): $f_n(x)=\sin(n^2x)/n$ converges uniformly to zero on $[-1,1]$, while $f_n'(0)=n$. The small amplitude does not control the slopes of the [sine](sine.md) oscillations.

## ↑ Ancestors (7)

1. [Uniform convergence](uniform-convergence.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/3g/solution.md)
- [Pointwise convergence](pointwise-convergence.md)
- [Uniform convergence](uniform-convergence.md)
