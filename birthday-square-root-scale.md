# Birthday square-root scale

↑ **Parent:** [Birthday problem](birthday-problem.md)

The [union bound](boole-s-inequality.md) gives $P_{n,m}\leq\min(1,n(n-1)/(2m))$. Using $1-x\leq e^{-x}$ on the distinct-label product gives

$$
1-e^{-n(n-1)/(2m)}\leq P_{n,m}\leq\min\left(1,\frac{n(n-1)}{2m}\right).
$$

The lower bound reaches at least one half when $n(n-1)/(2m)\geq\log2$. The simple approximation $n\approx\sqrt{2m\log2}$ predicts a group size near 23 for $m=365$. It is the quadratic number of pairs that makes the [square root](square-root.md) appear.

For a precise limiting statement, let $m\to\infty$ and $n/\sqrt m\to c\geq0$. Expanding the [logarithm](logarithm.md) of the complement yields

$$
\log(1-P_{n,m})=-\frac{n(n-1)}{2m}+O\left(\frac{n^3}{m^2}\right),\qquad
P_{n,m}\longrightarrow1-e^{-c^2/2}.
$$

On this scale the remainder tends to zero. Thus a fixed substantial collision probability appears after order $\sqrt m$ draws. For $m=2^b$ uniform output labels, the corresponding scale is order $2^{b/2}$; [matching one specified birthday](matching-one-specified-birthday.md) instead involves a number of draws of order $m$.

## ↑ Ancestors (5)

1. [Birthday problem](birthday-problem.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Birthday problem](birthday-problem.md)
