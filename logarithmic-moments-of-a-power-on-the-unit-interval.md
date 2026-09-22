# Logarithmic moments of a power on the unit interval

↑ **Parent:** [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)

For real $m>-1$ and integer $n\geq0$, start from $\int_0^1x^m\,dx=1/(m+1)$ and differentiate $n$ times with respect to $m$. Each derivative adds one factor $\log x$, giving

$$
\int_0^1x^m(\log x)^n\,dx=\frac{(-1)^nn!}{(m+1)^{n+1}}.
$$

To justify [differentiation under the integral sign](differentiation-under-the-integral-sign.md), restrict $m$ to a compact interval with lower endpoint $m_0>-1$. The derivatives are dominated by $x^{m_0}|\log x|^n$, which is integrable: $x=e^{-t}$ turns its integral into $\int_0^\infty e^{-(m_0+1)t}t^n\,dt$. A [power](power.md) of $t$ is integrable against this decaying exponential. This also explains why $m=-1$ is the convergence threshold.

## ↑ Ancestors (5)

1. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/20/b/solution.md)
