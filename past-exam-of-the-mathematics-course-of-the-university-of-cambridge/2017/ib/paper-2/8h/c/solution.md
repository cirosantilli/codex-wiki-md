<h1 id="8h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $U_{(1)}=\min(U_1,U_2)$ and $U_{(2)}=\max(U_1,U_2)$ be the [order statistics](../../../../../../order-statistic.md). For the symmetric [uniform distribution](../../../../../../continuous-uniform-distribution.md), each observation is above or below $\theta$ with probability $1/2$, independently. Thus

$$
\mathbb P_\theta\{U_{(1)}\le\theta\le U_{(2)}\}
=1-(1/2)^2-(1/2)^2=1/2.
$$

So $\boxed{[U_{(1)},U_{(2)}]}$ is an exact 50% [confidence interval](../../../../../../confidence-interval.md).

The observed interval $[10,11.5]$ contains values impossible under the sampling model. Both observations must lie within one unit of the parameter, so the interval of all compatible values is $[U_{(2)}-1,U_{(1)}+1]=[10.5,11]$. It contains the true parameter almost surely. A [support-restricted confidence interval for a uniform location parameter](../../../../../../support-restricted-confidence-interval-for-a-uniform-location-parameter.md) can therefore report

$$
\boxed{[10.5,11].}
$$

More precisely, the procedure $[U_{(1)},U_{(2)}]\cap[U_{(2)}-1,U_{(1)}+1]$ retains exact 50% unconditional coverage, since the second interval contains $\theta$ almost surely. The intersection is a nonempty interval for every sample in the model and equals $[10.5,11]$ for these data. Reporting the full compatible interval alone is also valid and has coverage one. On this sample's large-spread event it lies wholly between the observations; this does not turn the unconditional 50% procedure into a generally 100% procedure.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8H](../../8h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
