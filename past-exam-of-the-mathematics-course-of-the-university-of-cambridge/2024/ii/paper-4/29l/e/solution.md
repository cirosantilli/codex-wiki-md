<h1 id="29l/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The average log price is

$$
\frac1T\int_0^T\log S_tdt
=\log S_0+\frac12\left(r-\frac12\sigma^2\right)T
+\frac\sigma T I_T.
$$

Part (b) gives $\operatorname{var}(I_T)=T^3/3$, so the Gaussian variance of the final term is

$$
v=\frac13\sigma^2T.
$$

Rewriting the lognormal factor in the normalized form $e^{-v/2+\sqrt vZ}$ and discounting gives

$$
S_0e^{-(r/2+\sigma^2/12)T}
F\left(\frac13\sigma^2T,
\frac{Ke^{-(r/2-\sigma^2/12)T}}{S_0}\right).
$$

**Thus $\alpha=1/12$.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [29L](../../29l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
