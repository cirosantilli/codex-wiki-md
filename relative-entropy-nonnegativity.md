# Relative entropy nonnegativity

↑ **Parent:** [Kullback-Leibler divergence](kullback-leibler-divergence.md)

For [probability distributions](probability-distribution.md) $P,Q$, [relative entropy](kullback-leibler-divergence.md) satisfies $D_{\mathrm{KL}}(P\Vert Q)\geq0$, with equality exactly when $P=Q$. Thus truthful prediction uniquely minimizes expected [log-loss](logarithmic-loss.md) whenever the comparison is well defined, explaining the [strictly proper scoring rule](strictly-proper-scoring-rule.md) property of the [logarithmic scoring rule](logarithmic-scoring-rule.md).

For a short proof with [probability density functions](probability-density-function.md) $f,g$ and $g>0$, set $r=f/g$. Their [integrals](integral.md) both equal one, giving

$$
H(f\mid g)=\int g\bigl(r\log r-r+1\bigr)\,d\mu\geq0.
$$

The [strictly convex function](strictly-convex-function.md) $r\log r-r+1$ is minimized only at $r=1$, so equality means $f=g$ [almost everywhere](almost-everywhere.md). Its value at zero is one by $0\log0=0$. Where $g=0<f$, [relative entropy](kullback-leibler-divergence.md) is infinite; where both vanish, the contribution is zero. These conventions extend the argument beyond positive reference [probability density functions](probability-density-function.md).

## ↑ Ancestors (6)

1. [Kullback-Leibler divergence](kullback-leibler-divergence.md)
2. [f-divergence](f-divergence.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Information projection](information-projection.md)
- [Kullback-Leibler divergence](kullback-leibler-divergence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-8/3/c/solution.md)
- [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md)
- [Total correlation](total-correlation.md)
