<h1 id="1/1/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Expanding the stable autoregressive inverse gives the [infinite moving-average representation](../../../../../../../infinite-moving-average-representation.md) in [linear innovations](../../../../../../../linear-innovation-process.md):

$$
\frac{1-B/3}{1-B/4}=1+\sum_{j\geq1}\left(4^{-j}-\tfrac13\,4^{-(j-1)}\right)B^j
=1-\sum_{j\geq1}\frac{B^j}{3\cdot4^j}.
$$

Therefore

$$
\boxed{X_t=\varepsilon_t-\sum_{j\geq1}\frac{\varepsilon_{t-j}}{3\cdot4^j}.}
$$

For comparison, the causal representation in the originally supplied noise is

$$
\boxed{X_t=\eta_t-11\sum_{j\geq1}4^{-j}\eta_{t-j}.}
$$

Both converge in $L^2$, since their coefficients are square summable. The second is causal, but its driving noise is not the linear [innovation process](../../../../../../../innovation-process.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
