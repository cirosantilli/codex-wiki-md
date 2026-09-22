<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\kappa=2(1-H)$ and fix $a>0$. Starting with part (b), the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) under the map $q\mapsto q/a$ gives an LDP for $r(X)/(aN)$ with speed $N^\kappa$ and [rate function](../../../../../../rate-function.md) $q\mapsto J(aq)$.

Alternatively, replace $N$ by $aN$ in parts (a) and (b), using the real-scale justification in part (a). The same family has [large-deviation speed](../../../../../../large-deviation-speed.md) $(aN)^\kappa$ and [rate function](../../../../../../rate-function.md) $J(q)$. When expressed at speed $N^\kappa$, that [rate function](../../../../../../rate-function.md) is $a^\kappa J(q)$. The two descriptions of the same [large deviation principle](../../../../../../large-deviation-principle.md) must agree:

$$
J(aq)=a^\kappa J(q).
$$

For clarity, uniqueness here is a general property of [lower semicontinuous](../../../../../../lower-semicontinuity.md) [rate functions](../../../../../../rate-function.md): at a point $x$, the shrinking-neighborhood logarithmic bounds recover $I(x)$, since $\inf_{B(x,\eta)}I\to I(x)$ as $\eta\downarrow0$. Thus two [rate functions](../../../../../../rate-function.md) for the same family and speed cannot differ.

Taking the base argument $q=1$ and replacing $a$ by any positive [queue](../../../../../../queue-queueing-theory.md) size gives

$$
\boxed{J(q)=q^{2(1-H)}J(1)\quad(q>0),\qquad J(0)=0.}
$$

For $q<0$ the [rate function](../../../../../../rate-function.md) is infinite. In the usual nondegenerate case $J(1)$ is finite, so the formula also holds at $q=0$. This is the [self-similar Gaussian workload rate](../../../../../../self-similar-gaussian-workload-rate.md); the exponent comes from the [Hurst parameter](../../../../../../hurst-exponent.md), while the constant comes from the path [rate function](../../../../../../rate-function.md) and the drift and noise scales.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
