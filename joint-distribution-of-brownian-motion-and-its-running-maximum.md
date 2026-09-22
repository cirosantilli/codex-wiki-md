# Joint distribution of Brownian motion and its running maximum

↑ **Parent:** [Brownian running maximum](brownian-running-maximum.md)

Let $M_t=\sup_{0\leq s\leq t}B_s$ for a standard [Brownian motion](brownian-motion-split.md). For $m\geq0$, the [Brownian reflection principle](reflection-principle-wiener-process.md) gives

$$
\mathbb P(B_t\leq b,M_t\leq m)=
\begin{cases}
\Phi(b/\sqrt t)+\Phi((2m-b)/\sqrt t)-1,&b\leq m,\\
2\Phi(m/\sqrt t)-1,&b>m.
\end{cases}
$$

On $b<m$, the pair $(B_t,M_t)$ therefore has [joint probability density](joint-probability-density.md)

$$
f_{B_t,M_t}(b,m)=
\frac{2(2m-b)}{\sqrt{2\pi}\,t^{3/2}}
e^{-(2m-b)^2/(2t)}.
$$

## ↑ Ancestors (9)

1. [Brownian running maximum](brownian-running-maximum.md)
2. [Reflection principle (Wiener process)](reflection-principle-wiener-process.md)
3. [Brownian motion](brownian-motion-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26/3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/29k/b/ii/solution.md)
