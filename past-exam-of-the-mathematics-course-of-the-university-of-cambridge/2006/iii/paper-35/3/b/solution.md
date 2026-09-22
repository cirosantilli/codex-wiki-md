<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the common [filtration](../../../../../../filtration-probability-theory.md) in which the two driving processes are independent [Brownian motions](../../../../../../brownian-motion-split.md) and the solutions are [adapted](../../../../../../adapted-process.md). Let $Z=X+Y$, and define [predictable](../../../../../../predictable-process.md) bounded weights

$$
h_1=\mathbf1_{\{Z>0\}}\sqrt{X/Z}+\mathbf1_{\{Z=0\}},\qquad
h_2=\mathbf1_{\{Z>0\}}\sqrt{Y/Z},
$$

with the ratios defined only on $\{Z>0\}$. The nonnegative solutions have $X=Y=0$ when $Z=0$. Set

$$
B_t=\int_0^t h_1(s)dB_s^{(1)}+\int_0^t h_2(s)dB_s^{(2)}.
$$

Independent Brownian drivers have zero cross-variation. Since $h_1^2+h_2^2=1$ even on the zero set, $[B]_t=t$, and the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes $B$ a [Brownian motion](../../../../../../brownian-motion-split.md). Moreover $\sqrt Z h_1=\sqrt X$ and $\sqrt Z h_2=\sqrt Y$ everywhere. Adding the two original equations therefore proves [additivity of independently driven squared Bessel processes](../../../../../../additivity-of-independently-driven-squared-bessel-processes.md):

$$
\boxed{dZ_t=2\sqrt{Z_t}\,dB_t+(\alpha+\beta)dt,\qquad \gamma=\alpha+\beta.}
$$

The unit-vector fill on $\{Z=0\}$ is essential: simply dividing by $\sqrt Z$ there would leave the Brownian construction undefined.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
