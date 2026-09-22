<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the shape-rate convention for the [gamma distribution](../../../../../../gamma-distribution.md). A shape $r$ and rate $\beta$ give [expected value](../../../../../../expected-value.md) $r/\beta$ and [variance](../../../../../../variance-split.md) $r/\beta^2$. The two moments here force $r=2$ and $\beta=2/\mu$. Thus $M_X(t)=\beta^2/(\beta-t)^2$, and the [geometric-sum moment-generating function](../../../../../../geometric-sum-moment-generating-function.md) becomes

$$
M_S(t)=\frac{p\beta^2}{(\beta-t)^2-(1-p)\beta^2}.
$$

Put $r_0=\sqrt{1-p}$, $a=\beta(1-r_0)$ and $b=\beta(1+r_0)$. Then $0<a<b$, $ab=p\beta^2$, and

$$
M_S(t)=\frac{a}{a-t}\frac{b}{b-t}\qquad(t<a).
$$

Consequently the [geometric sum of shape-two gamma variables](../../../../../../geometric-sum-of-shape-two-gamma-variables.md) has the same [probability distribution](../../../../../../probability-distribution.md) as the sum of two independent [exponential distributions](../../../../../../exponential-distribution.md) with rates $a,b$. Their [convolution of independent random variables](../../../../../../convolution-of-independent-random-variables.md) yields

$$
\boxed{f_S(s)=\frac{ab}{b-a}(e^{-as}-e^{-bs})
=\frac{p}{\mu\sqrt{1-p}}
\left(e^{-2(1-\sqrt{1-p})s/\mu}-e^{-2(1+\sqrt{1-p})s/\mu}\right),\quad s>0.}
$$

The [probability density function](../../../../../../probability-density-function.md) is zero for $s<0$. It is nonnegative because $a<b$, and its integral is

$$
\frac{ab}{b-a}\left(\frac1a-\frac1b\right)=1.
$$

This verifies normalization directly. An alternative check uses the conditional [gamma distribution](../../../../../../gamma-distribution.md) with shape $2n$:

$$
\sum_{n\geq1}p(1-p)^{n-1}\frac{\beta^{2n}s^{2n-1}e^{-\beta s}}{(2n-1)!}
=\frac{p\beta}{r_0}e^{-\beta s}\sinh(\beta r_0s),
$$

which is exactly the same density. The [expected value](../../../../../../expected-value.md) $1/a+1/b=\mu/p$ supplies a further check.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
