<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

As printed, the requested conclusion is false for $\delta\ne1$. On an interval on which $X$ stays positive, the [time change of a continuous process](../../../../../../time-change-of-a-continuous-process.md) satisfies $d\tau_s=ds/(\delta^2X_s^{2(\delta-1)/\delta})$. The time-changed martingale term has [quadratic variation](../../../../../../quadratic-variation.md) $s$, so the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) identifies it with a standard Brownian motion $\widetilde B$. Dividing the drift in part (a) by the derivative of the clock gives

$$
\frac{\frac{\delta(\delta-1)}2X_s^{(\delta-2)/\delta}}{\delta^2X_s^{2(\delta-1)/\delta}}=\frac{\delta-1}{2\delta X_s}.
$$

Consequently the construction actually satisfies

$$
dX_s=\frac{\delta-1}{2\delta X_s}ds+d\widetilde B_s,
$$

which is the [Bessel process](../../../../../../bessel-process.md) equation of dimension $2-1/\delta$. It equals the paper's claimed drift $(\delta-1)/(2X_s)$ only when $\delta=1$. The mismatch between the specified power, clock, and conclusion is therefore a typographical error in the question.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
