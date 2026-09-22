<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [expected value](../../../../../../../expected-value-split.md) of a signed [random variable](../../../../../../../random-variable-split.md) is finite precisely when its absolute value is [integrable](../../../../../../../integrability.md). With the [standard normal distribution](../../../../../../../standard-normal-distribution.md) [probability density function](../../../../../../../probability-density-function.md),

$$
\mathbb E|Ze^{\alpha Z^2}|
=\frac2{\sqrt{2\pi}}\int_0^\infty z\exp\bigl[-(1/2-\alpha)z^2\bigr]\,dz.
$$

For $\alpha<1/2$, this [integral](../../../../../../../integral-split.md) equals $1/[\sqrt{2\pi}(1/2-\alpha)]<\infty$. For $\alpha\ge1/2$, its [integrand](../../../../../../../integrand.md) does not decay sufficiently and the [integral](../../../../../../../integral-split.md) diverges. Therefore

$$
\boxed{\mathbb E[Ze^{\alpha Z^2}]\text{ exists exactly for }\alpha<\frac12,
\quad\text{and then equals }0.}
$$

The value is zero by the [odd function](../../../../../../../odd-function.md) and the [symmetric distribution](../../../../../../../symmetric-distribution.md). For the other $\alpha$, both positive and negative parts have infinite [integrals](../../../../../../../integral-split.md); formal cancellation would give only a [Cauchy principal value](../../../../../../../cauchy-principal-value.md), not an [expected value](../../../../../../../expected-value-split.md). This distinction is the [integrability threshold for exponential powers of a Gaussian](../../../../../../../integrability-threshold-for-exponential-powers-of-a-gaussian.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
