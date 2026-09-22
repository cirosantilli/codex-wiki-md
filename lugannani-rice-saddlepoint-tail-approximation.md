# Lugannani-Rice saddlepoint tail approximation

↑ **Parent:** [Saddlepoint density approximation](saddlepoint-density-approximation.md)

For a sample mean from an independent identically distributed sample, let $K(t)$ be the [cumulant-generating function](cumulant-generating-function.md) of one observation and solve $K'(t)=x$. Put $w=\operatorname{sgn}(t)\sqrt{2n(tx-K(t))}$ and $u=t\sqrt{nK''(t)}$. Under the smooth, nonlattice conditions for a [saddlepoint density approximation](saddlepoint-density-approximation.md), the corresponding approximation to the [cumulative distribution function](cumulative-distribution-function.md) is

$$
\Pr(\overline X\le x)\simeq\Phi(w)+\phi(w)\left(\frac1w-\frac1u\right),
$$

where $\Phi$ and $\phi$ are the standard [normal distribution](normal-distribution.md) functions. The apparent singularity at $t=0$ is removable. Write $v=K''(0)$ and $k=K'''(0)$; [Taylor expansion](taylor-expansion.md) gives $w=t\sqrt{nv}(1+kt/(3v)+O(t^2))$ and $u=t\sqrt{nv}(1+kt/(2v)+O(t^2))$. Thus $1/w-1/u\to k/(6\sqrt n\,v^{3/2})$. The approximation requires suitable tail regularity and is not a universal formula for distributions without a moment-generating function.

## ↑ Ancestors (9)

1. [Saddlepoint density approximation](saddlepoint-density-approximation.md)
2. [Cumulant-generating function](cumulant-generating-function.md)
3. [Moment-generating function](moment-generating-function.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/6/i/solution.md)
