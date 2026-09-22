# Isolating a logarithmic singularity to test a power-series endpoint

↑ **Parent:** [Radius of convergence](radius-of-convergence.md)

Suppose $A\ne0$ and $R>0$, and $H$ is an [analytic function](holomorphic-function-split.md) on a disk of radius strictly larger than $R$. The [Taylor series](taylor-series.md) at zero of $f(z)=A\log(1-z/R)+H(z)$ has [radius of convergence](radius-of-convergence.md) $R$. Its coefficients are the sum of $-A/(nR^n)$ and the more rapidly decreasing coefficients of $H$. At $x=-R$, the logarithmic part is an alternating [harmonic series](harmonic-series.md) and converges conditionally; at $x=R$ it diverges. The [power series](power-series.md) for $H$ converges absolutely at both endpoints and therefore cannot change either conclusion. The real convergence interval is $[-R,R)$.

For $f(z)=\log(2-e^z)$, take $R=\log2$ and $H(z)=\log[(2-e^z)/(1-z/R)]$, with its branch normalized by $H(0)=0$. The quotient has nonzero removable value $2R$ at $z=R$. Its next zeros are at $R\pm2\pi i$, so a [holomorphic logarithm](holomorphic-logarithm.md) exists on a larger disk. This shows why the [Taylor series](taylor-series.md) converges at $x=-\log2$ even though its singular positive endpoint is excluded.

## ↑ Ancestors (8)

1. [Radius of convergence](radius-of-convergence.md)
2. [Power series](power-series.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/15/d/solution.md)
