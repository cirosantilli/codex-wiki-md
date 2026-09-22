# Sine-weighted power integral recurrence

↑ **Parent:** [Integration by parts](integration-by-parts.md)

Define the [definite integral](definite-integral.md) $F(k)=\int_0^\pi x^k\sin x\,dx$. For real $k>1$, two applications of [integration by parts](integration-by-parts.md) give

$$
F(k)=\pi^k+k\int_0^\pi x^{k-1}\cos x\,dx
=\pi^k-k(k-1)F(k-2).
$$

The boundary term $x^{k-1}\sin x$ vanishes at both endpoints. At $k=1$, direct integration gives $F(1)=\pi$, consistent with the displayed relation; $F(-1)$ is finite because $\sin x/x\to1$ at zero. This recurrence and $F(0)=2$ evaluate every nonnegative integer moment, with separate even and odd chains.

## ↑ Ancestors (7)

1. [Integration by parts](integration-by-parts.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/17/c/solution.md)
