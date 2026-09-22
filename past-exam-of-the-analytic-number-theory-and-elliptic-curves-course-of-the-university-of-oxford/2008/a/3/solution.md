<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Each finite-interval integral $f_n(s)$ is entire in $s$: the integrand is $ (x-n)e^{-(s+1)\log x}$ and its complex derivatives may be integrated on the compact interval. On a compact subset of $\operatorname{Re}s>0$, choose $\delta>0$ with $\operatorname{Re}s\ge\delta$. Then $|f_n(s)|\le n^{-1-\delta}$. The Weierstrass uniform-convergence theorem gives convergence and holomorphy of $\sum_nf_n(s)$ throughout that half-plane.

[Integration by parts](../../../../integration-by-parts.md) gives

$$
sf_n(s)=-(n+1)^{-s}+\int_n^{n+1}x^{-s}\,dx.
$$

For $\operatorname{Re}s>1$, sum absolutely and use the integral over $[1,\infty)$ to obtain $s\sum_nf_n(s)=1-\zeta(s)+1/(s-1)$. Rearranging gives the first requested identity.

On $[n,n+1]$, the magnitude of $(x-n)(x-n-1)$ is at most $1/4$. On a compact subset of $\operatorname{Re}s>-1$, its integrals are bounded by a convergent constant multiple of $n^{-1-\delta}$ for some $\delta>0$. Thus $\sum_ng_n(s)$ is [holomorphic](../../../../holomorphic-function-split.md) there. The prefactor $s(s+1)$ is entire, leaving only the explicit [simple pole](../../../../simple-pole.md) at one in $\widetilde\zeta$, with [residue](../../../../residue.md) one.

Differentiate $(x-n)(x-n-1)x^{-s-1}$ and integrate. Its endpoint values both vanish, giving

$$
\boxed{(s+1)g_n(s)-2f_n(s)=-\int_n^{n+1}x^{-s-1}\,dx=\frac{(n+1)^{-s}-n^{-s}}s.}
$$

At $s=0$ the last quotient has its continuous value $-\log((n+1)/n)$. For $\operatorname{Re}s>1$, telescoping over $n$ gives $(s+1)\sum_ng_n-2\sum_nf_n=-1/s$. Substitution into $\widetilde\zeta$ yields

$$
\widetilde\zeta(s)=\frac1{s-1}+1-s\sum_nf_n(s)=\frac s{s-1}-s\sum_nf_n(s)=\zeta(s).
$$

This supplies the [analytic continuation](../../../../analytic-continuation.md) to $\operatorname{Re}s>-1$ apart from the [pole](../../../../pole.md). Evaluating its [holomorphic](../../../../holomorphic-function-split.md) expression at zero makes the series term vanish and gives $\boxed{\zeta(0)=-1/2}$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
