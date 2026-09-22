<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Normal-normal conjugacy](../../../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives

$$
p(\theta\mid y)=N(\widetilde\theta,\sigma_\theta^2),
\qquad
\sigma_\theta^2=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2},
\qquad
\widetilde\theta=\frac{\tau^2}{\sigma^2+\tau^2}y.
$$

The three quantities in the proposed identity are

$$
\log Z=-\frac12\left[
\log(2\pi(\sigma^2+\tau^2))+
\frac{y^2}{\sigma^2+\tau^2}
\right],
$$



$$
\mathbb E_{\theta\mid y}\log L(\theta)
=-\frac12\log(2\pi\sigma^2)
-\frac{(y-\widetilde\theta)^2+\sigma_\theta^2}{2\sigma^2},
$$

and, by the [Kullback-Leibler divergence between normal distributions](../../../../../../../kullback-leibler-divergence-between-normal-distributions.md),

$$
D_{\mathrm{KL}}(p(\theta\mid y)\Vert\pi)
=\frac12\left[
\log\frac{\tau^2}{\sigma_\theta^2}
+\frac{\sigma_\theta^2+\widetilde\theta^2}{\tau^2}-1
\right].
$$

Substitution and simplification show that the latter two expressions differ by exactly $\log Z$, so the equality holds.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
