<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed real $t$, [Taylor's theorem](../../../../../taylor-s-theorem.md) for the [exponential function](../../../../../exponential-function.md) gives

$$
e^{t/\sqrt{k}}=1+\frac t{\sqrt{k}}+\frac{t^2}{2k}+O(k^{-3/2}).
$$

Substituting into the previous [moment-generating function](../../../../../moment-generating-function.md),

$$
\log M_{Y_k}(t)=\frac{t^2}{2}+O(k^{-1/2}),\qquad
M_{Y_k}(t)\longrightarrow e^{t^2/2}.
$$

The [continuity theorem for moment-generating functions](../../../../../convergence-theorem-for-moment-generating-functions.md) states that, if the [moment-generating functions](../../../../../moment-generating-function.md) of $Z_n$ and $Z$ are finite on a common open [interval](../../../../../interval-mathematics.md) containing zero and $M_{Z_n}(t)\to M_Z(t)$ throughout that interval, then $Z_n\xrightarrow{\mathrm d}Z$. Here finiteness holds for all real $t$, and the limit is the [moment-generating function of a standard normal variable](../../../../../moment-generating-function-of-a-standard-normal-variable.md). Therefore

$$
\boxed{Y_k\xrightarrow{\mathrm d}N(0,1).}
$$

This proves the required instance of the [Poisson central limit theorem](../../../../../poisson-central-limit-theorem.md) directly from [moment-generating functions](../../../../../moment-generating-function.md); no appeal to a general [central limit theorem](../../../../../central-limit-theorem.md) is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
