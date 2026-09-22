# Sine sequence is not Cauchy in the integral norm

↑ **Parent:** [Lp space](lp-space.md)

On $[0,1]$, the [continuous functions](continuous-function.md) $f_n(x)=\sin(nx)$ do not form a [Cauchy sequence](cauchy-sequence.md) in the [Lp space](lp-space.md) with $p=1$. Put $d_n=f_n-f_{2n}$. The identity $\int_0^1d_n^2\,dx=1-\sin(2n)/(4n)-\sin(4n)/(8n)-\sin n/n+\sin(3n)/(3n)$ tends to $1$. Since $|d_n|\leq2$, one has $\int_0^1|d_n|\,dx\geq\frac12\int_0^1d_n^2\,dx$, which stays bounded away from zero. Thus arbitrarily late pairs are separated in the integral [norm](norm.md); in particular the sequence cannot converge in that [norm](norm.md).

## ↑ Ancestors (7)

1. [Lp space](lp-space.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/13h/solution.md)
