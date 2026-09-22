# Contraction estimate on a shrinking holomorphic domain

↑ **Parent:** [Weighted holomorphic norm on a shrinking time domain](weighted-holomorphic-norm-on-a-shrinking-time-domain.md)

Write $N=\|u\|_\alpha$, $r=|t|$ and $A=\alpha(1-s)>r$. Along the straight integration segment, choose $\sigma(\tau)=s+(A-\tau)/(2\alpha)$. A [Cauchy estimate](cauchy-estimate.md) on a disc of radius $R(\sigma-s)$ bounds the integrand by $4\alpha N\tau/[R(A-\tau)^2]$. Therefore

$$
\frac{A-r}{r}\left|\int_0^t\partial_xu(x,z)\,dz\right|
\leq\frac{4\alpha N}{R}\left[1+\frac{A-r}{r}\log(1-r/A)\right]
\leq\frac{4\alpha N}{R}.
$$

The integral is taken at fixed $x$, and the disc and segment lie inside the shrinking domain. Consequently $u\mapsto\int_0^t(iu_x+f)\,dz$ is a [contraction mapping](contraction-mapping.md) when $0<\alpha<R/4$ and the holomorphic source $f$ is bounded on the relevant closed polydisc. The source term has weighted norm at most $\alpha\sup|f|$, so the [Banach fixed-point theorem](contraction-mapping-theorem.md) gives a holomorphic solution with zero initial data.

## ↑ Ancestors (8)

1. [Weighted holomorphic norm on a shrinking time domain](weighted-holomorphic-norm-on-a-shrinking-time-domain.md)
2. [Space of holomorphic functions](space-of-holomorphic-functions.md)
3. [Holomorphic function](holomorphic-function.md)
4. [Complex analysis](complex-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105/1/iii/solution.md)
