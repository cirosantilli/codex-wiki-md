<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the random-walk proposal specified by its centre and [covariance](../../../../../../covariance.md): for the current state $z=(x,y)$ draw $Z_1,Z_2$ independently standard normal and set

$$
x'=x+\sigma_qZ_1,\qquad y'=y+\sigma_qZ_2,\qquad\sigma_q>0.
$$

Its properly normalized density of the [proposal distribution](../../../../../../proposal-distribution.md) is

$$
q(z'\mid z)=\frac1{2\pi\sigma_q^2}\exp\left(-\frac{(x'-x)^2+(y'-y)^2}{2\sigma_q^2}\right).
$$

It is symmetric: $q(z'\mid z)=q(z\mid z')$. This is a centred-at-the-current-state proposal, rather than an unshifted draw from the density notation in the source. The [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md) consequently needs only the target ratio. Put $H(x,y)=x^2+y^2-2\rho xy$. Then

$$
\boxed{\alpha(z,z')=\min\left\{1,\exp\left(-\frac{H(x',y')-H(x,y)}{2(1-\rho^2)}\right)\right\}.}
$$

An [independent](../../../../../../independent-random-variables.md) uniform decides the move; on rejection both coordinates remain at their previous values. A proposal with lower $H$ is always accepted. This construction uses the joint density directly, without needing either [conditional distribution](../../../../../../conditional-distribution.md). Its continuous positive proposal density supplies communication over the target support, and the holding probability avoids a deterministic periodic transition pattern.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
