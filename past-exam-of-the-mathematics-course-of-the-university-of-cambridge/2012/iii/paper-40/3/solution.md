<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [classical risk model](../../../../../classical-risk-model.md) surplus $U_t=u+ct-\sum_{j=1}^{N_t}X_j$, with $c>0$, and write $\varphi$ for its ultimate [survival probability](../../../../../survival-probability.md). The [first-claim decomposition for survival probability](../../../../../first-claim-decomposition-for-survival-probability.md) follows by conditioning on the first arrival time of the [Poisson process](../../../../../poisson-process.md). That time has [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$. A claim at time $t$ leaves capital $u+ct-x$ if $x\leq u+ct$, after which the [Markov property](../../../../../markov-property.md) restarts the same risk model. Consequently

$$
\varphi(u)=\int_0^\infty\lambda e^{-\lambda t}
\int_0^{u+ct}\varphi(u+ct-x)f(x)\,dx\,dt.
$$

Put $C(v)=\int_0^v\varphi(v-x)f(x)\,dx$ and change variable $v=u+ct$:

$$
\varphi(u)=\frac\lambda c e^{\lambda u/c}
\int_u^\infty e^{-\lambda v/c}C(v)\,dv.
$$

The [convolution](../../../../../convolution.md) $C$ is continuous since $\varphi$ is bounded and $f$ is integrable. Differentiating proves the [survival integro-differential equation](../../../../../survival-integro-differential-equation-for-a-classical-risk-model.md)

$$
\boxed{\varphi'(u)=\frac\lambda c\varphi(u)-\frac\lambda c
\int_0^u\varphi(u-x)f(x)\,dx,\qquad a_1=\lambda/c,\quad a_2=-\lambda/c.}
$$

For the specified claim law, expand its [probability density function](../../../../../probability-density-function.md) as $f(x)=\tfrac12e^{-x}+\tfrac14e^{-x/2}$. This is an equal-weight [mixture distribution](../../../../../mixture-distribution.md) of [exponential distributions](../../../../../exponential-distribution.md) with rates $1$ and $1/2$. In the [convolution](../../../../../convolution.md), set $z=u-x$ to obtain

$$
C(u)=\frac12e^{-u}I_1(u)+\frac14e^{-u/2}I_2(u).
$$

Since $\lambda/c=10/21$, the requested coefficients are

$$
\boxed{b_1=\frac{10}{21},\qquad b_2=-\frac5{21},\qquad b_3=-\frac5{42}.}
$$

For the [exponential-mixture differential equation for survival probability](../../../../../exponential-mixture-differential-equation-for-survival-probability.md), define $A(u)=e^{-u}I_1(u)$, $B(u)=e^{-u/2}I_2(u)$ and $r=\lambda/c$. Differentiating the integrals yields

$$
A'=\varphi-A,\qquad B'=\varphi-\tfrac12B,\qquad
\varphi'=r\varphi-\tfrac r2A-\tfrac r4B.
$$

Apply $(D+1)(D+\tfrac12)$ to the last equation, where $D=d/du$. The first two equations eliminate $A,B$, giving

$$
\varphi'''+\frac32\varphi''+\frac12\varphi'
=r\varphi''+\frac{3r}{4}\varphi'.
$$

Thus

$$
\boxed{\varphi'''+\frac{43}{42}\varphi''+\frac17\varphi'=0,
\qquad c_1=43/42,\quad c_2=1/7.}
$$

The [characteristic polynomial](../../../../../characteristic-polynomial.md) factors as

$$
D\left(D^2+\frac{43}{42}D+\frac17\right)
=D(D+\tfrac16)(D+\tfrac67).
$$

The [ordinary differential equation](../../../../../ordinary-differential-equation.md) therefore has solution $C_0+C_1e^{-u/6}+C_2e^{-6u/7}$.

The claim [expected value](../../../../../expected-value.md) is $\tfrac12\cdot1+\tfrac12\cdot2=3/2$. The [relative safety loading](../../../../../relative-safety-loading.md) is $\rho=2.1/(3/2)-1=2/5$, and the given [zero-capital survival probability](../../../../../zero-capital-survival-probability.md) is $\varphi(0)=2/7$. The limit at infinity sets $C_0=1$. A third condition comes from the original [survival integro-differential equation](../../../../../survival-integro-differential-equation-for-a-classical-risk-model.md): its [convolution](../../../../../convolution.md) vanishes at zero, so $\varphi'(0)=(10/21)(2/7)=20/147$. Therefore

$$
C_1+C_2=-\frac57,\qquad
-\frac{C_1}{6}-\frac{6C_2}{7}=\frac{20}{147},
$$

which gives $C_1=-20/29$ and $C_2=-5/203$. The final [survival probability](../../../../../survival-probability.md) and [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) are

$$
\boxed{\varphi(u)=1-\frac{20}{29}e^{-u/6}-\frac5{203}e^{-6u/7},}
$$



$$
\boxed{\psi(u)=\frac{20}{29}e^{-u/6}+\frac5{203}e^{-6u/7}\qquad(u\geq0).}
$$

Both exponential coefficients of $\psi$ are positive. Hence $\varphi$ increases from $2/7$ to one, and $\psi$ decreases from $5/7$ to zero. The initial slope is essential: the two stated boundary values alone do not determine all three constants of the eliminated differential equation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
