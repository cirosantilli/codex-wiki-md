<h1 id="question-6/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

For a nonzero separable solution of the [Laplace equation in polar coordinates](../../../../../../laplace-equation-in-polar-coordinates.md), write $T(r,\theta)=R(r)\Theta(\theta)$ with $r>0$. Multiplying the [partial differential equation](../../../../../../partial-differential-equation-split.md) by $r^2$ and dividing where $R\Theta\ne0$ gives

$$
\frac{r^2R''+rR'}R=-\frac{\Theta''}{\Theta}=\lambda,
$$

where $\lambda$ is a real [separation constant](../../../../../../separation-constant.md). The resulting [ordinary differential equations](../../../../../../ordinary-differential-equation.md) are

$$
r^2R''+rR'-\lambda R=0,\qquad\Theta''+\lambda\Theta=0.
$$

The equations continue across zeros of the factors by continuity. The radial equation is a [Cauchy-Euler equation](../../../../../../cauchy-euler-equation.md); putting $s=\log r$ changes it to $d^2R/ds^2-\lambda R=0$.

For **positive separation constant**, write $\lambda=k^2$ with $k>0$. The radial factors are powers, while the angular factors are [sine](../../../../../../sine.md) and [cosine](../../../../../../cosine.md):

$$
\boxed{T=(A r^k+B r^{-k})(C\cos(k\theta)+D\sin(k\theta))}.
$$

For **zero separation constant**, each transformed equation has zero second [derivative](../../../../../../derivative.md), giving

$$
\boxed{T=(A+B\log r)(C+D\theta)}.
$$

For **negative separation constant**, write $\lambda=-k^2$ with $k>0$. The radial factors oscillate in $\log r$, and the angular factors are [exponential functions](../../../../../../exponential-function.md):

$$
\boxed{T=(A\cos(k\log r)+B\sin(k\log r))(C e^{k\theta}+D e^{-k\theta})}.
$$

These exhaust the nonzero real separated solutions before imposing angular [periodicity](../../../../../../periodicity.md) or regularity at the origin. The zero solution is also allowed. Since [Laplace's equation](../../../../../../laplace-equation.md) is linear, sums of these separated solutions are solutions wherever the sums and required [derivatives](../../../../../../derivative.md) converge appropriately.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
