<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a nearby orbit, linearized separation satisfies $\delta_{i+1}=f'(x_i)\delta_i$. Repeated use of the [chain rule](../../../../../chain-rule.md) gives $\delta_n=\delta_0\prod_{i=0}^{n-1}f'(x_i)$ to first order. Taking the logarithm of its magnitude and dividing by $n$ gives the exponential growth rate

$$
\boxed{\lambda=\lim_{n\to\infty}\frac1n\log\left|\frac{\delta_n}{\delta_0}\right|=\lim_{n\to\infty}\frac1n\sum_{i=0}^{n-1}\log|f'(x_i)|.}
$$

The infinitesimal-perturbation limit is taken before interpreting long-time growth; finite separations eventually leave the linear regime. The limit is assumed to exist, with a limsup used when needed.

On a $p$-cycle, blocks of $p$ successive [derivatives](../../../../../derivative.md) repeat. If $M=(f^p)'(x_0)=\prod_{i=0}^{p-1}f'(x_i)$, the remainder of fewer than $p$ terms has vanishing contribution to the long-time average and

$$
\boxed{\lambda=\frac1p\log|M|.}
$$

Linear attraction means $|M|<1$, giving $\lambda<0$. A superstable cycle has $M=0$, meaning at least one [derivative](../../../../../derivative.md) in the cycle vanishes. Its infinitesimal return multiplier is zero and the corresponding logarithmic exponent is $-\infty$. This concerns the [derivative](../../../../../derivative.md) cocycle; actual finite perturbations can converge by higher-order rather than literally vanishing in one step.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
