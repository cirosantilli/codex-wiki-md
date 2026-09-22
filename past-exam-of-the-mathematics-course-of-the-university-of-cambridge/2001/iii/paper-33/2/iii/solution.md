<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here the proposal is $Y=x+\eta$ with $\eta\sim N_2(0,I_2)$. Its [probability density function](../../../../../../probability-density-function.md) depends only on $\|y-x\|^2$, so $q(y\mid x)=q(x\mid y)$. The determinant and [normalizing constant](../../../../../../normalizing-constant.md) of the target also cancel. With $Q$ as in the preceding entry,

$$
\boxed{\alpha(x,y)=\min\{1,e^{-[Q(y)-Q(x)]/2}\}.}
$$

Equivalently, writing $u_j=(y_j-\mu_j)/\sigma_j$ and $z_j=(x_j-\mu_j)/\sigma_j$,

$$
\alpha(x,y)=\min\!\left\{1,
\exp\!\left[-\frac{
u_1^2-2\rho u_1u_2+u_2^2-z_1^2+2\rho z_1z_2-z_2^2
}{2(1-\rho^2)}\right]\right\}.
$$

One can also compute the exponent without subtracting two large [quadratic forms](../../../../../../quadratic-form.md):

$$
\log\frac{\pi(x+\eta)}{\pi(x)}
=-\eta^\top\Sigma^{-1}(x-\mu)-\frac12\eta^\top\Sigma^{-1}\eta.
$$

Generate two [independent](../../../../../../independent-random-variables.md) [standard normal distribution](../../../../../../standard-normal-distribution.md) proposal increments, compute this log ratio, and accept when $\log U\leq\min(0,\log(\pi(Y)/\pi(x)))$. Retain the previous pair on rejection. [Detailed balance](../../../../../../detailed-balance.md) gives the correct [invariant distribution](../../../../../../stationary-distribution.md), and the everywhere-positive [Gaussian](../../../../../../normal-distribution.md) proposal makes this [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md) chain irreducible; a rejection [probability](../../../../../../probability.md) provides a holding step. The resulting target-distributed pairs are dependent, with proposal scale and target anisotropy controlling how quickly they mix.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
