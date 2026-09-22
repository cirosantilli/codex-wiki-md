# Integrating a mean-zero periodic function divided by x

↑ **Parent:** [Improper integral](improper-integral.md)

Let $h$ be measurable, integrable over a positive period $L$, and have mean zero there. Its positive and negative parts have equal integrals $H$. On the $k$-th period the signed integral of $h(x)/x$ has absolute value at most

$$
\frac H L\left(\frac1k-\frac1{k+1}\right).
$$

This follows by bounding the positive and negative weighted integrals between $H/((k+1)L)$ and $H/(kL)$. The bounds are summable, so the integrals at period endpoints converge. A leftover partial period has absolute integral at most $\|h\|_{L^1(0,L)}/(kL)$, tending to zero, which proves convergence for arbitrary upper endpoints too.

In contrast, each full-period integral of $|h(x)|/x$ is at least $2H/((k+1)L)$. It diverges in total unless $H=0$, equivalently $h=0$ almost everywhere. Thus a nonzero mean-zero periodic function gives a convergent improper integral here but no [Lebesgue integrability](integrability.md).

## ↑ Ancestors (8)

1. [Improper integral](improper-integral.md)
2. [Riemann integral](riemann-integral.md)
3. [Riemann integration](riemann-integration.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/d/d3/b/ii/solution.md)
