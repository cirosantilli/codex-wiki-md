<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $N=\lfloor x\rfloor$, interchange a finite sum and an integral:

$$
\int_1^x S(t)F'(t)\,dt
=\sum_{n\le x}f(n)\int_n^x F'(t)\,dt
=F(x)S(x)-\sum_{n\le x}f(n)F(n).
$$

This proves the [Abel's summation formula](../../../../abel-s-summation-formula.md), including the term at $n=1$.

Apply it with $f(n)=1$, $F(t)=1/t$. Writing $\{t\}=t-\lfloor t\rfloor$ gives

$$
H_{\lfloor x\rfloor}=\log x+1-\frac{\{x\}}x-\int_1^x\frac{\{t\}}{t^2}\,dt
=\log x+\gamma-\frac{\{x\}}x+\int_x^\infty\frac{\{t\}}{t^2}\,dt.
$$

The last two terms are $O(x^{-1})$, proving the first expansion. For the refinement let $B_1(t)=\{t\}-1/2$. It has mean [zero](../../../../zero-of-a-function.md) on each unit interval, so its [primitive](../../../../primitive-group-action.md) $P(t)=\int_0^tB_1(u)\,du$ is bounded and periodic. [Integration by parts](../../../../integration-by-parts.md) gives

$$
\int_x^\infty\frac{B_1(t)}{t^2}\,dt
=-\frac{P(x)}{x^2}+2\int_x^\infty\frac{P(t)}{t^3}\,dt=O(x^{-2}).
$$

Thus for [integer](../../../../integer-split.md) $x$, where $\{x\}=0$,

$$
\boxed{H_x=\log x+\gamma+\frac1{2x}+O(x^{-2}).}
$$

For the zeta representation, integrating each defining integral by parts yields

$$
sf_n(s)=-(n+1)^{-s}+\frac{(n+1)^{1-s}-n^{1-s}}{1-s}.
$$

Summing from $1$ to $N-1$ and substituting into the definition of $\zeta$ gives

$$
\boxed{\zeta(s)=\frac{N^{1-s}}{s-1}+\sum_{n\le N}n^{-s}-s\sum_{n=N}^\infty f_n(s).}
$$

Since $0\le x-n\le1$,

$$
\left|\sum_{n=N}^\infty f_n(s)\right|
\le\sum_{n=N}^\infty\int_n^{n+1}x^{-\sigma-1}\,dx
=\frac{N^{-\sigma}}\sigma.
$$

This is uniform on compact subsets of $\operatorname{Re}s>0$, so the series is [holomorphic](../../../../holomorphic-function-split.md) there and limits at $s=1$ are legitimate after subtracting the [pole](../../../../pole.md). Expanding $N^{1-s}=1-(s-1)\log N+O((s-1)^2)$ gives

$$
a_0=H_N-\log N-\sum_{n=N}^\infty f_n(1).
$$

The final tail is $O(N^{-1})$, and the harmonic expansion sends the remaining difference to $\gamma$. Therefore

$$
\boxed{a_0=\gamma.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
