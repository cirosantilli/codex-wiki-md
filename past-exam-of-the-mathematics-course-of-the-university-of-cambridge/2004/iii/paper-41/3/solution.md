<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For nontrivial positive [claim sizes](../../../../../claim-size.md) in the [classical risk model](../../../../../classical-risk-model.md) and $\lambda>0$, the [adjustment coefficient](../../../../../adjustment-coefficient.md) is the unique positive solution

$$
\boxed{\lambda(M_X(R)-1)=cR,\qquad 0<R<r_\infty.}
$$

Indeed, $h(r)=\lambda(M_X(r)-1)-cr$ has $h(0)=0$, $h'(0)=\lambda\mu-c<0$, and is [strictly convex](../../../../../strictly-convex-function.md). It becomes positive near the right endpoint of the [moment-generating function](../../../../../moment-generating-function.md) domain. For a finite endpoint this follows from the assumed divergence; for an infinite endpoint, $\mathbb P(X\ge\varepsilon)>0$ for some $\varepsilon>0$ gives an exponential lower bound on $M_X(r)$, which eventually exceeds any linear function. [Convexity](../../../../../convex-function.md) gives existence and uniqueness of the positive crossing and $\lambda M_X'(R)-c>0$.

Put $q=\lambda\mu/c$ and $\overline F=1-F$. Substituting $\varphi=1-\psi$ into the supplied [survival renewal equation for a classical risk model](../../../../../survival-renewal-equation-for-a-classical-risk-model.md), and using $\int_0^\infty\overline F(x)dx=\mu$, yields

$$
\psi(u)=\frac{\lambda}{c}\int_u^\infty\overline F(x)\,dx
+\frac{\lambda}{c}\int_0^u\psi(u-x)\overline F(x)\,dx.
$$

Multiplying by $e^{Ru}$ gives the proper renewal-type equation

$$
\boxed{Z(u)=g_R(u)+\int_0^u Z(u-x)k_R(x)\,dx,}
\qquad
k_R(x)=\frac{\lambda}{c}e^{Rx}\overline F(x),\quad
g_R(u)=\frac{\lambda}{c}e^{Ru}\int_u^\infty\overline F(x)\,dx.
$$

The [exponential tilt of the ruin renewal kernel](../../../../../exponential-tilt-of-the-ruin-renewal-kernel.md) turns a defective kernel into a [probability density function](../../../../../probability-density-function.md), because the tail integration identity gives

$$
\int_0^\infty k_R(x)dx
=\frac{\lambda}{c}\frac{M_X(R)-1}{R}=1.
$$

This identity follows also by integrating $e^{RX}-1=R\int_0^X e^{Rx}dx$ and applying [Tonelli theorem](../../../../../tonelli-theorem.md). The tilted [probability density function](../../../../../probability-density-function.md) defines a [nonarithmetic distribution](../../../../../nonarithmetic-distribution.md), even if the [claim size](../../../../../claim-size.md) [probability distribution](../../../../../probability-distribution.md) itself has atoms.

Differentiate $(M_X(R)-1)/R$ to calculate its [mean](../../../../../expected-value.md):

$$
m_R=\int_0^\infty xk_R(x)dx
=\frac{\lambda}{c}\frac{RM_X'(R)-M_X(R)+1}{R^2}
=\frac{\lambda M_X'(R)-c}{cR}.
$$

It is finite and positive because $R$ is inside the finite [moment-generating function](../../../../../moment-generating-function.md) domain. Next, reversing the order of integration gives

$$
\begin{aligned}
\int_0^\infty g_R(u)du
&=\frac{\lambda}{c}\int_0^\infty\overline F(x)\int_0^x e^{Ru}du\,dx\\
&=\frac{\lambda}{cR}\left(\frac{M_X(R)-1}{R}-\mu\right)
=\frac{c-\lambda\mu}{cR}.
\end{aligned}
$$

The forcing function is [directly Riemann integrable](../../../../../direct-riemann-integrability.md). Choose $\varepsilon>0$ with $M_X(R+\varepsilon)<\infty$. [Markov's inequality](../../../../../markov-inequality.md) bounds $\overline F(x)$ by $M_X(R+\varepsilon)e^{-(R+\varepsilon)x}$, so $g_R(u)$ is bounded by a constant times $e^{-\varepsilon u}$. It is continuous; on finite intervals continuity controls its [Riemann sums](../../../../../riemann-sum.md), and the exponential envelope controls the tails. These are sufficient conditions for [direct Riemann integrability](../../../../../direct-riemann-integrability.md).

Iterating the [renewal equation](../../../../../renewal-equation.md) by [convolution](../../../../../convolution.md) gives $Z=g_R*U_R$, where $U_R=\sum_{n\ge0}k_R^{*n}$ is the [renewal measure](../../../../../renewal-measure.md). The remainder after $n$ iterations is bounded on each fixed interval by a constant times the chance that a sum of $n$ positive interarrivals remains in that interval, which tends to zero. The [key renewal theorem](../../../../../key-renewal-theorem.md), applicable to this [nonarithmetic distribution](../../../../../nonarithmetic-distribution.md) of finite [mean](../../../../../expected-value.md) and the directly integrable forcing, now gives the [interior adjustment coefficient ruin prefactor](../../../../../interior-adjustment-coefficient-ruin-prefactor.md):

$$
\boxed{A=\lim_{u\to\infty}e^{Ru}\psi(u)
=\frac{\int_0^\infty g_R(u)du}{m_R}
=\frac{c-\lambda\mu}{\lambda M_X'(R)-c}.}
$$

Both numerator and denominator are positive, so $0<A<\infty$.

For the unit-rate shape-two [Erlang distribution](../../../../../erlang-distribution.md), $\mu=2$, $M_X(r)=(1-r)^{-2}$ and $M_X'(r)=2(1-r)^{-3}$. Write $\delta=\lambda/c$, so positive loading requires $0<\delta<1/2$. Dividing the [adjustment coefficient](../../../../../adjustment-coefficient.md) equation by its nonzero root gives $\delta(2-R)=(1-R)^2$. Thus

$$
\boxed{R=1-\frac{\delta+\sqrt{\delta^2+4\delta}}2,\qquad
A=\frac{1-2\delta}{2\delta(1-R)^{-3}-1}
=\frac{(1-R)(3-2R)}{3-R}.}
$$

The last simplification uses $\delta=(1-R)^2/(2-R)$; it is the [Erlang shape-two ruin prefactor](../../../../../erlang-shape-two-ruin-prefactor.md). Its value depends on the premium-to-arrival ratio, which is not specified numerically.

For the final exponential representation, evaluating at zero in the [survival renewal equation for a classical risk model](../../../../../survival-renewal-equation-for-a-classical-risk-model.md) gives **$\lambda\mu/c=\psi(0)=a+b$**. If the slower term is present, necessarily $a>0$ and $e^u\psi(u)\to a$. Comparing with the finite positive asymptotic constant just proved yields

$$
\boxed{R=1,\qquad A=a,\qquad\lambda\mu/c=a+b\quad(a>0).}
$$

A smaller [adjustment coefficient](../../../../../adjustment-coefficient.md) would make the limit zero and a larger one would make it infinite. Here the [leading exponential term determines a ruin adjustment coefficient](../../../../../leading-exponential-term-determines-a-ruin-adjustment-coefficient.md). The coefficient $b$ need not be assumed positive to identify the leading term.

The wording does not specify that $a$ is nonzero. If $a=0$ and $b>0$, the only surviving term instead gives **$R=6$, $A=b$ and $\lambda\mu/c=b$**. This case is realizable: claims with an [exponential distribution](../../../../../exponential-distribution.md) of rate $\beta=6+\lambda/c$ have [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) $(\lambda/(c\beta))e^{-6u}$. Negative $a$ would make the [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) negative for large $u$, and both coefficients zero are incompatible with a nontrivial positive claim rate and [mean](../../../../../expected-value.md). These observations specify the coefficient qualification needed for the usual $R=1$ answer.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
