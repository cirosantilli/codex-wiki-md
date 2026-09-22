<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [classical risk model](../../../../../classical-risk-model.md), write the surplus as

$$
U(t)=u+ct-\sum_{j=1}^{N(t)}X_j,\qquad c=(1+\theta)\lambda\mu,
$$

where $N(t)$ is the claim-arrival [Poisson process](../../../../../poisson-process.md). The ruin time is $\tau=\inf\{t\ge0:U(t)<0\}$. The [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) is

$$
\boxed{\psi(u)=\mathbb P(\tau<\infty).}
$$

The positive root $R$ in the question is the [adjustment coefficient](../../../../../adjustment-coefficient.md). The [Lundberg inequality](../../../../../lundberg-inequality.md) and the [Cramér–Lundberg approximation](../../../../../cramer-lundberg-ruin-asymptotic.md) are, respectively,

$$
\boxed{\psi(u)\le e^{-Ru},}
\qquad
\boxed{\psi(u)\sim C e^{-Ru}\quad(u\to\infty),\qquad
 C=\frac{\theta\mu}{M_X'(R)-(1+\theta)\mu}.}
$$

The [interior adjustment coefficient ruin prefactor](../../../../../interior-adjustment-coefficient-ruin-prefactor.md) is finite here because $R$ lies strictly inside the finite domain of the [moment-generating function](../../../../../moment-generating-function.md); the claim-size density supplies the nonarithmetic condition for the asymptotic. Strict convexity makes its denominator positive. The approximation is an asymptotic statement, while the inequality is a bound at every nonnegative initial capital.

The inequality can also be seen directly from the [exponential surplus martingale](../../../../../exponential-surplus-martingale.md) $e^{-RU(t)}$. Its expectation factor per unit time is zero in the exponent because $\lambda(M_X(R)-1)-cR=0$. Apply the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $\tau\wedge T$, a bounded time. On $\{\tau\le T\}$, $e^{-RU(\tau)}>1$, so $\mathbb P(\tau\le T)\le e^{-Ru}$. Increasing $T$ proves the bound without stopping at an unbounded time.

For any nonnegative claim size, the [Tonelli theorem](../../../../../tonelli-theorem.md) applied to $e^{RX}-1=\int_0^X Re^{Rx}\,dx$ gives the exponential tail identity

$$
M_X(R)-1=R\int_0^\infty e^{Rx}(1-F_X(x))\,dx.
$$

Combining it with the adjustment equation yields

$$
\boxed{\frac1\mu\int_0^\infty e^{Rx}(1-F_X(x))\,dx=1+\theta.}
$$

The density $f_Y(x)=(1-F_X(x))/\mu$ integrates to one by the [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md). Thus $Y$ has the [equilibrium claim-size distribution](../../../../../equilibrium-claim-size-distribution.md), and the preceding formula says $M_Y(R)=1+\theta$.

Under the given [NBUE](../../../../../new-better-than-used-in-expectation.md) condition, the [stochastic order](../../../../../stochastic-order.md) comparison is $1-F_Y(x)\le1-F_X(x)$ at every $x\ge0$. Apply the same exponential tail identity to both variables to obtain

$$
\mathbb E e^{RY}=1+R\int_0^\infty e^{Rx}(1-F_Y(x))\,dx
\le1+R\int_0^\infty e^{Rx}(1-F_X(x))\,dx
=\mathbb E e^{RX}.
$$

Consequently

$$
1+\theta=M_Y(R)\le M_X(R)=1+(1+\theta)\mu R,
$$

and rearrangement proves the [adjustment-coefficient lower bound for NBUE claims](../../../../../adjustment-coefficient-lower-bound-for-nbue-claims.md):

$$
\boxed{R\ge\frac{\theta}{(1+\theta)\mu}.}
$$

This uses the specified distributional comparison, not an unwarranted assumption that an arbitrary equilibrium claim law is always smaller than its original law.

For the final example, $f_X(x)=xe^{-x}$ is the shape-two, rate-one [gamma distribution](../../../../../gamma-distribution.md), with $\mu=2$, survival function $\overline F_X(x)=(1+x)e^{-x}$, and [moment-generating function](../../../../../moment-generating-function.md) $M_X(r)=(1-r)^{-2}$ for $r<1$. With $\theta=1/10$, the positive adjustment root satisfies

$$
(1-R)^{-2}-1=\frac{11}{5}R.
$$

Dividing out the zero root and simplifying gives $11R^2-17R+1=0$. Only the smaller root is in the finite-transform interval $(0,1)$, so

$$
\boxed{R=\frac{17-7\sqrt5}{22}\approx0.0612511.}
$$

The equilibrium density and survival function are

$$
f_Y(x)=\frac{(1+x)e^{-x}}2,\qquad
\overline F_Y(x)=\frac12\int_x^\infty(1+t)e^{-t}\,dt
=(1+x/2)e^{-x}.
$$

Thus $\overline F_Y(x)\le(1+x)e^{-x}=\overline F_X(x)$ for every $x\ge0$, proving that this claim law is [new better than used in expectation](../../../../../new-better-than-used-in-expectation.md). Finally the lower bound equals $1/22$. Our exact root is larger because $16>7\sqrt5$, equivalently $256>245$. Hence

$$
\boxed{R>\frac1{22}\approx0.0454545,}
$$

verifying the requested bound for the example.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
