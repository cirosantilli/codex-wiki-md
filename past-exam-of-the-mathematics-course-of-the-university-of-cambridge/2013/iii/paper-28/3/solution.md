<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [classical risk model](../../../../../classical-risk-model.md) write $U(t)=u+ct-\sum_{j=1}^{N(t)}X_j$, where the [Poisson process](../../../../../poisson-process.md) $N(t)$ has rate $\lambda$ and is independent of the claim sizes. Define the ruin time and ultimate [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) by

$$
\tau_u=\inf\{t\ge0:U(t)<0\},\qquad\psi(u)=\mathbb P(\tau_u<\infty),\quad u\ge0.
$$

The [relative safety loading](../../../../../relative-safety-loading.md) is $\rho=c/(\lambda\mu)-1>0$, so $c=(1+\rho)\lambda\mu$. The [adjustment coefficient](../../../../../adjustment-coefficient.md) is the nonzero positive solution

$$
\boxed{\lambda\{M(R)-1\}=cR.}
$$

Existence and uniqueness follow from the [secant-slope existence criterion for an adjustment coefficient](../../../../../secant-slope-existence-criterion-for-an-adjustment-coefficient.md). Explicitly, $\lambda(M(r)-1)-cr$ has derivative $\lambda\mu-c<0$ at zero and is strictly convex for positive claims. The assumed divergence of $M$ makes it cross zero once at a positive $R<r_\infty$. When $r_\infty=\infty$, an exponential lower bound from any positive tail event shows that $M(r)/r\to\infty$. In particular $R$ is inside the finite-transform domain, not at its endpoint.

Put $\overline F=1-F$. Replacing $\varphi=1-\psi$ in the [survival renewal equation for a classical risk model](../../../../../survival-renewal-equation-for-a-classical-risk-model.md) yields

$$
\psi(u)=\frac{\lambda}{c}\left(\mu-\int_0^u\overline F(x)\,dx\right)+\frac{\lambda}{c}\int_0^u\psi(u-x)\overline F(x)\,dx.
$$

By the [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md), $\mu=\int_0^\infty\overline F(x)\,dx$. Therefore this is the [defective renewal equation](../../../../../defective-renewal-equation.md)

$$
\psi(u)=\frac\lambda c\int_u^\infty\overline F(x)\,dx+\frac\lambda c\int_0^u\psi(u-x)\overline F(x)\,dx.
$$

The original kernel has mass $\lambda\mu/c=1/(1+\rho)<1$. For the [exponential tilt of the ruin renewal kernel](../../../../../exponential-tilt-of-the-ruin-renewal-kernel.md), set

$$
k_R(x)=\frac\lambda c e^{Rx}\overline F(x),\qquad
h_R(u)=\frac\lambda c e^{Ru}\int_u^\infty\overline F(x)\,dx.
$$

Multiplying by $e^{Ru}$ gives the required proper [renewal equation](../../../../../renewal-equation.md)

$$
\boxed{Z(u)=h_R(u)+\int_0^u Z(u-x)k_R(x)\,dx,\qquad Z(u)=e^{Ru}\psi(u).}
$$

To verify that this is a probability renewal kernel, [Tonelli theorem](../../../../../tonelli-theorem.md) gives, for $r>0$ in the finite-transform domain,

$$
\int_0^\infty e^{rx}\overline F(x)\,dx=\mathbb E\int_0^X e^{rx}\,dx=\frac{M(r)-1}{r}.
$$

The [adjustment coefficient](../../../../../adjustment-coefficient.md) equation consequently implies $\int_0^\infty k_R(x)\,dx=1$. Its [expected value](../../../../../expected-value.md) is

$$
m_R=\int_0^\infty xk_R(x)\,dx
=\frac\lambda c\frac{RM'(R)-(M(R)-1)}{R^2}
=\frac{\lambda M'(R)-c}{cR}.
$$

It is finite because $R$ is interior to the finite-transform domain and is positive because the strict convex crossing has derivative $\lambda M'(R)-c>0$.

We quote the [key renewal theorem](../../../../../key-renewal-theorem.md) in the following form: for a [nonarithmetic distribution](../../../../../nonarithmetic-distribution.md) $K$ of positive increments with finite positive mean $m$, and a [directly Riemann integrable](../../../../../direct-riemann-integrability.md) nonnegative function $h$, the locally bounded solution of $z=h+z*K$ satisfies $z(u)\to m^{-1}\int_0^\infty h$. It has [renewal representation](../../../../../renewal-representation.md) $z=h*\sum_{j\ge0}K^{*j}$; this follows by iterating the equation, since the probability that arbitrarily many positive increments have sum at most a fixed $u$ tends to zero.

Here $K_R(dx)=k_R(x)\,dx$ is absolutely continuous, and hence [nonarithmetic distribution](../../../../../nonarithmetic-distribution.md), even if the original claim law has atoms. The function $h_R$ is continuous. Choose $\delta>0$ with $M(R+\delta)<\infty$. The [Markov inequality](../../../../../markov-inequality.md) gives $\overline F(x)\le M(R+\delta)e^{-(R+\delta)x}$, and hence $h_R(u)\le C_\delta e^{-\delta u}$. Continuity on compact intervals and this exponential bound make the upper Riemann sums finite with uniformly vanishing tails, proving [direct Riemann integrability](../../../../../direct-riemann-integrability.md).

A further application of [Tonelli theorem](../../../../../tonelli-theorem.md) evaluates the forcing integral:

$$
\begin{aligned}
\int_0^\infty h_R(u)\,du
&=\frac\lambda c\int_0^\infty\overline F(x)\int_0^x e^{Ru}\,du\,dx\\
&=\frac\lambda{cR}\left(\frac{M(R)-1}{R}-\mu\right)
=\frac{c-\lambda\mu}{cR}.
\end{aligned}
$$

All hypotheses of the [key renewal theorem](../../../../../key-renewal-theorem.md) are now checked, so the [interior adjustment coefficient ruin prefactor](../../../../../interior-adjustment-coefficient-ruin-prefactor.md) is

$$
\boxed{\lim_{u\to\infty}e^{Ru}\psi(u)=\frac{c-\lambda\mu}{\lambda M'(R)-c}
=\frac{\rho\mu}{M'(R)-(1+\rho)\mu}.}
$$

This proves the requested [Cramér–Lundberg ruin asymptotic](../../../../../cramer-lundberg-ruin-asymptotic.md), including its constant.

For the two-component [hyperexponential distribution](../../../../../hyperexponential-distribution.md), conditioning on the chosen exponential component gives

$$
\overline F(x)=\frac12 e^{-x}+\frac12 e^{-x/2},\quad x\ge0,
\qquad
\boxed{\mu=\frac32.}
$$

Its [moment-generating function](../../../../../moment-generating-function.md) and derivative are

$$
M(r)=\frac1{2(1-r)}+\frac1{2(1-2r)},\qquad
M'(r)=\frac1{2(1-r)^2}+\frac1{(1-2r)^2},\quad r<\frac12.
$$

The [moment-generating function](../../../../../moment-generating-function.md) diverges at $1/2$, while the derivative of the adjustment equation at zero is negative. Strict convexity therefore places its unique positive [adjustment coefficient](../../../../../adjustment-coefficient.md) in

$$
\boxed{0<R<\frac12.}
$$

The adjustment equation, divided by $R$, becomes

$$
\frac1{2(1-R)}+\frac1{1-2R}=\frac32(1+\rho).
$$

Using this identity to subtract $(1+\rho)\mu$ from $M'(R)$ gives

$$
M'(R)-\frac32(1+\rho)=\frac{R}{2(1-R)^2}+\frac{2R}{(1-2R)^2}.
$$

Thus the asymptotic constant in terms of $\rho$ and $R$ is

$$
\boxed{\lim_{u\to\infty}e^{Ru}\psi(u)
=\frac{3\rho}{R\{(1-R)^{-2}+4(1-2R)^{-2}\}}.}
$$

The denominator is positive on the identified domain. If desired, $R$ is the smaller root of $6(1+\rho)R^2-(5+9\rho)R+3\rho=0$; the other algebraic root lies outside the positive finite-transform interval and is not an [adjustment coefficient](../../../../../adjustment-coefficient.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
