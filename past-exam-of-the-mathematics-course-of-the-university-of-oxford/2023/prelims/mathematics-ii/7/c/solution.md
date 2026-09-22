<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The functions $g_n$ are nonnegative. The [change of variables](../../../../../../change-of-variables-formula.md) $u=nx$ and the given [Gaussian integral](../../../../../../gaussian-integral.md) imply

$$
M_n:=\int_0^1g_n(x)\,dx=\frac2{\sqrt\pi}\int_0^n e^{-u^2}\,du\longrightarrow1,
\qquad 0\leq M_n\leq1.
$$

For every fixed $\delta>0$,

$$
\int_\delta^1g_n(x)\,dx\leq\frac2{\sqrt\pi}\int_{n\delta}^\infty e^{-u^2}\,du\longrightarrow0.
$$

Thus the mass concentrates at the endpoint zero. This is a [one-sided approximate identity](../../../../../../one-sided-approximate-identity.md).

Because $f$ is [continuous](../../../../../../continuous-function.md) on the [compact interval](../../../../../../compact-interval.md) $[0,1]$, it is a [bounded function](../../../../../../bounded-function.md); put $B=\sup_{[0,1]}|f|$. Given $\varepsilon>0$, choose $\delta\in(0,1)$ with $|f(x)-f(0)|<\varepsilon$ for $0\leq x<\delta$. Splitting the integral near and away from zero yields

$$
\begin{aligned}
\left|\int_0^1 f(x)g_n(x)\,dx-f(0)\right|
&\leq\int_0^1|f(x)-f(0)|g_n(x)\,dx+|f(0)|\,|M_n-1|\\
&\leq\varepsilon M_n+2B\int_\delta^1g_n(x)\,dx+|f(0)|\,|M_n-1|.
\end{aligned}
$$

Taking the [limit superior](../../../../../../limit-superior.md) gives a bound of $\varepsilon$, and $\varepsilon$ was arbitrary. Consequently

$$
\boxed{\int_0^1 f(x)g_n(x)\,dx\longrightarrow f(0).}
$$

Only [continuity](../../../../../../continuous-function.md) at zero and boundedness on $[0,1]$ were needed for this final estimate; the assumed [continuity](../../../../../../continuous-function.md) everywhere also guarantees the ordinary integrals exist.

## ↑ Ancestors (12)

1. [C](../c.md)
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
