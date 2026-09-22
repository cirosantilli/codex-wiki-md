# Small-ball conditioning for a Poisson random measure

↑ **Parent:** [Count-weighted Laplace functional of a Poisson random measure](count-weighted-laplace-functional-of-a-poisson-random-measure.md)

For a [Poisson random measure](poisson-random-measure.md) on $\mathbb R^d$ with [Lebesgue measure](lebesgue-measure.md) intensity and a nonnegative compactly supported [continuous function](continuous-function.md) $f$, put $m_r=\mu(B(0,r))$ and $a_r=\int_{B(0,r)}e^{-f}d\mu$. Continuity gives $a_r/m_r\to e^{-f(0)}$. With $L=\mathbb E e^{-M(f)}$, the [count-weighted Laplace functional of a Poisson random measure](count-weighted-laplace-functional-of-a-poisson-random-measure.md) and independent inside/outside counts give respectively

$$
\frac{\mathbb E[M(B(0,r))e^{-M(f)}]}{\mathbb P(M(B(0,r))\geq1)}=L\frac{a_r}{1-e^{-m_r}},\qquad
\mathbb E[e^{-M(f)}\mid M(B(0,r))\geq1]=L\frac{1-e^{-a_r}}{1-e^{-m_r}}.
$$

Both converge to the displayed value. The conditioning is meaningful for every $r>0$; it is not conditioning on a positive-probability point at the origin.

## ↑ Ancestors (9)

1. [Count-weighted Laplace functional of a Poisson random measure](count-weighted-laplace-functional-of-a-poisson-random-measure.md)
2. [Laplace functional of a Poisson random measure](laplace-functional-of-a-poisson-random-measure.md)
3. [Poisson random measure](poisson-random-measure.md)
4. [Poisson point process](poisson-point-process.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32/6/b/iii/solution.md)
