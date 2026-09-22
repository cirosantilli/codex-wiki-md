<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in the usual joint natural [filtration](../../../../../../../filtration-probability-theory.md) of $B$ and $W$, in which both are Brownian motions. The integrand is $\operatorname{sgn}(B_s)$, as printed in the PDF. It is [predictable](../../../../../../../predictable-process.md) and bounded, so $X$ is a zero-starting [continuous local martingale](../../../../../../../continuous-local-martingale.md). The [quadratic variation of a stochastic integral](../../../../../../../quadratic-variation-of-a-stochastic-integral.md) gives

$$
[X]_t=\int_0^t\operatorname{sgn}(B_s)^2\,ds=t.
$$

If the sign is defined to be zero at zero, the final equality still holds: [Tonelli's theorem](../../../../../../../tonelli-theorem.md) gives $\mathbb E\int_0^t\mathbf1_{\{B_s=0\}}ds=\int_0^t\mathbb P(B_s=0)ds=0$. Thus the Brownian zero set has zero Lebesgue time on every compact interval. The [Lévy characterization of Brownian motion](../../../../../../../levy-characterization-of-brownian-motion.md) proves that **$X$ is standard Brownian motion**. This is the [Brownian sign transform](../../../../../../../brownian-sign-transform.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
