<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $C_t=\int_0^tZ_s^2ds$ and $\tau_u=\inf\{t:C_t>u\}$. By the [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md), $W_u=M_{\tau_u}$ is Brownian motion. Setting $Y_u=Z_{\tau_u}$ and using $du=Z_t^2dt$ transforms the decomposition in part b into

$$
dY_u=dW_u+\frac{a+1/2}{Y_u}\,du.
$$

Comparison with the [Bessel process](../../../../../../bessel-process.md) equation $dY_u=dW_u+(d-1)(2Y_u)^{-1}du$ gives

$$
d=2a+2.
$$

**Thus an exponential Brownian motion with drift becomes a Bessel process under its quadratic-variation time change; this is an [Exponential Brownian-to-Bessel time change](../../../../../../exponential-brownian-to-bessel-time-change.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
