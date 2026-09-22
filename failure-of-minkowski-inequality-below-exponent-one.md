# Failure of Minkowski inequality below exponent one

↑ **Parent:** [Minkowski inequality](minkowski-inequality.md)

For $0<p<1$, write $Q_p(f)=(\int|f|^p\,d\mu)^{1/p}$ to emphasize that this is a [quasi-norm](quasi-norm.md), as in the [Lq quasi-norm](lq-quasi-norm.md) branch. On two coordinates with [counting measure](counting-measure.md), $u=(1,0)$ and $v=(0,1)$ give $Q_p(u)=Q_p(v)=1$, but $Q_p(u+v)=2^{1/p}>2$. At $p=1/2$, this is the explicit failure $4>1+1$ in the right panel of the diagram. The midpoint $(1/2,1/2)$ has $Q_p=2^{1/p-1}>1$, so the corresponding unit sublevel [set](set-split.md) is not a [convex set](convex-set.md).

A useful replacement survives: for nonnegative [real numbers](real-number.md) $a,b$, $(a+b)^p\leq a^p+b^p$. Together with the scalar [triangle inequality](triangle-inequality.md), this yields

$$
Q_p(f+g)^p\leq Q_p(f)^p+Q_p(g)^p.
$$

Consequently $d_p(f,g)=Q_p(f-g)^p$ is a [metric](metric.md) on the [equivalence classes](equivalence-class.md) of [measurable functions](measurable-function.md) with finite $Q_p$, even though $Q_p(f-g)$ itself need not be a [metric](metric.md). Do not replace the failed [Minkowski inequality](minkowski-inequality.md) by a universal reversed bound for signed or complex [functions](function-split.md): $g=-f\ne0$ would give a zero sum but two positive separate sizes.

## ↑ Ancestors (7)

1. [Minkowski inequality](minkowski-inequality.md)
2. [Lp norm](lp-norm.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
