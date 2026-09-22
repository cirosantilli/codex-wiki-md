<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One method applies [inverse transform sampling](../../../../../../inverse-transform-sampling.md) to the standard normal [cumulative distribution function](../../../../../../cumulative-distribution-function.md): $Z_i=\Phi^{-1}(U_i)$, followed by $X_i=\mu+\sigma Z_i$ for mean $\mu$ and [standard deviation](../../../../../../standard-deviation.md) $\sigma>0$. Numerical approximations to $\Phi^{-1}$ are needed, and the endpoints $U=0,1$ must be avoided.

A convenient alternative is the [Box-Muller transform](../../../../../../box-muller-transform.md). From independent uniforms $U_1,U_2\in(0,1)$ set

$$
R=\sqrt{-2\log U_1},\quad\Theta=2\pi U_2,\qquad
\boxed{Z_1=R\cos\Theta,\quad Z_2=R\sin\Theta.}
$$

The radial [probability density function](../../../../../../probability-density-function.md) is $re^{-r^2/2}$ for $r>0$, and the angle is independently uniform on $[0,2\pi)$. Dividing their joint density by the polar-coordinate [Jacobian determinant](../../../../../../jacobian-determinant.md) $r$ gives

$$
p(z_1,z_2)=\frac1{2\pi}e^{-(z_1^2+z_2^2)/2}
=\phi(z_1)\phi(z_2).
$$

Thus the outputs are independent standard [normal distribution](../../../../../../normal-distribution.md) draws. Apply $\mu+\sigma Z_j$ to obtain other normal means and [variances](../../../../../../variance-split.md). With finite [pseudorandom number generators](../../../../../../pseudorandom-number-generator.md), this is an approximation to the ideal independent-uniform model; poor dependence in the input stream is not cured by the transform.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
