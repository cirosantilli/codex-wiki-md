<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Draw independent $U_1,U_2$ uniformly on $(0,1)$, and set

$$
R=\sqrt{-2\log U_1},\qquad\Theta=2\pi U_2,
$$



$$
\boxed{X_1=R\cos\Theta,\qquad X_2=R\sin\Theta.}
$$

This is the [Box-Muller transform](../../../../../../box-muller-transform.md). The endpoint $U_1=0$ has probability zero; an implementation should avoid evaluating its logarithm.

For $r\geq0$, $P(R\leq r)=1-e^{-r^2/2}$, so $R$ has density $re^{-r^2/2}$. It is independent of the angle, which has a [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,2\pi)$, and their joint density is $(2\pi)^{-1}re^{-r^2/2}$. Transforming to Cartesian coordinates divides by the polar-coordinate Jacobian $r$, yielding

$$
f_{X_1,X_2}(x_1,x_2)=\frac1{2\pi}e^{-(x_1^2+x_2^2)/2}=\varphi(x_1)\varphi(x_2).
$$

Thus the outputs are [independent random variables](../../../../../../independent-random-variables.md) with the [standard normal distribution](../../../../../../standard-normal-distribution.md), proving the algorithm.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
