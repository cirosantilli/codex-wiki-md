<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The light-curve posterior used the analysis prior $\pi_0(\Delta t)=N(0,\sigma_{\mathrm{prior}}^2)$, so its marginal likelihood as a function of delay is proportional to $p(\Delta t\mid D)/\pi_0(\Delta t)$. Therefore

$$
p(H_0\mid D,M_l)\propto
\mathbf1_{[H_{0\min},H_{0\max}]}(H_0)
\int
\frac{p(\Delta t\mid D)}{\pi_0(\Delta t)}
p(\Delta t\mid H_0,M_l)\,d\Delta t.
$$

The integral can be evaluated numerically using the approximation from part (d).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
