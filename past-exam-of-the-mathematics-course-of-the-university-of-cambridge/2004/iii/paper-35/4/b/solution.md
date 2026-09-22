<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One route is [inverse transform sampling](../../../../../../inverse-transform-sampling.md): if $\Phi$ is the standard normal [cumulative distribution function](../../../../../../cumulative-distribution-function.md), then $\mu+\sigma\Phi^{-1}(U)$ has the [normal distribution](../../../../../../normal-distribution.md) with mean $\mu$ and [variance](../../../../../../variance-split.md) $\sigma^2$.

Alternatively the [Box-Muller transform](../../../../../../box-muller-transform.md) uses two independent uniform inputs $U_1,U_2\in(0,1)$:

$$
\boxed{Z_1=\sqrt{-2\log U_1}\cos(2\pi U_2),\qquad Z_2=\sqrt{-2\log U_1}\sin(2\pi U_2).}
$$

To verify this, set $R=\sqrt{-2\log U_1}$ and $\Theta=2\pi U_2$. The radial density is $re^{-r^2/2}$ for $r>0$, and the angle is independent and uniform. Their joint density is $re^{-r^2/2}/(2\pi)$. Changing to Cartesian coordinates divides by the [Jacobian determinant](../../../../../../jacobian-determinant.md) $r$, giving

$$
f_{Z_1,Z_2}(x,y)=\frac1{2\pi}e^{-(x^2+y^2)/2}.
$$

This factors into two standard normal densities, proving both normality and independence. Then $\mu+\sigma Z_j$ provides the required means and variances. Implementations must avoid the zero input to the logarithm; ideal continuous uniforms hit it with probability zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
