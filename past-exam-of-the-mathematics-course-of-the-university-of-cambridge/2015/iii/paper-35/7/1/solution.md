<h1 id="7/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $T=\min(T_A,T_B)$ be the first event time and $J$ its type. The [cause-specific hazard](../../../../../../cause-specific-hazard.md) for A is

$$
h_A(t)=\lim_{u\downarrow0}\frac{\Pr(t\leq T<t+u,\ J=A\mid T\geq t)}u.
$$

It is a rate among people free of both event types, not the marginal probability of eventually experiencing A. Under the given [independent](../../../../../../independent-random-variables.md) latent event times, their constant [hazard functions](../../../../../../hazard-function.md) give exponential [survivor functions](../../../../../../survival-function.md). Therefore **the first-event survivor is**

$$
\boxed{S(t)=\Pr(T_A\geq t,T_B\geq t)
=e^{-\alpha t}e^{-\beta t}=e^{-(\alpha+\beta)t}.}
$$

The combined first-event rate is $s=\alpha+\beta>0$. Subsequent formulas concerning conditioning on type A require $\alpha>0$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [7](../../7.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
