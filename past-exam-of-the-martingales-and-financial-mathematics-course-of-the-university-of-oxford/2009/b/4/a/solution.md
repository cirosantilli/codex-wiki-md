<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô's formula](../../../../../ito-s-lemma.md) to $\log X$ for positive initial value $x_0$. The drift correction is $-\sigma^2/2$, so

$$
\boxed{X_t=x_0\exp\{(\mu-\tfrac12\sigma^2)t+\sigma W_t\}.}
$$

This is [geometric Brownian motion](../../../../../geometric-brownian-motion.md). Under the physical probability measure, $W_T/\sqrt T$ has the [standard normal distribution](../../../../../standard-normal-distribution.md). For positive volatility,

$$
\boxed{\mathbb P(X_T<m)=\Phi\left(\frac{\log(m/x_0)-(\mu-\sigma^2/2)T}{\sigma\sqrt T}\right).}
$$

The drift here is $\mu$, because this is a physical bankruptcy probability. The [risk-neutral measure](../../../../../risk-neutral-measure.md) will instead give drift $r$ for pricing. If $\sigma=0$, the value is deterministic and the default probability is the indicator of $x_0e^{\mu T}<m$; the usual positive-volatility convention is used in the remaining formulas.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
