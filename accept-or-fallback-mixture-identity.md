# Accept-or-fallback mixture identity

↑ **Parent:** [Law of total probability](law-of-total-probability.md)

Let a [discrete random variable](discrete-random-variable.md) $Y$ have [probability mass function](probability-mass-function.md) $p_y$. Given $Y=y$, return $y$ with [probability](probability.md) $a_y\in[0,1]$; otherwise draw from a [conditional distribution](conditional-distribution.md) with [probability mass function](probability-mass-function.md) $K(y,x)$. The [law of total probability](law-of-total-probability.md) gives the displayed identity. Its total mass is $\sum_yp_y[a_y+(1-a_y)\sum_xK(y,x)]=1$. If the fallback is a [discrete uniform distribution](discrete-uniform-distribution.md) on $0,\ldots,y$, then $K(y,x)=\mathbf1_{\{0\leq x\leq y\}}/(y+1)$, so the fallback sum includes $y=x$.

## ↑ Ancestors (8)

1. [Law of total probability](law-of-total-probability.md)
2. [Probability measure](probability-measure.md)
3. [Probability space](probability-space-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/2/b/ii/solution.md)
