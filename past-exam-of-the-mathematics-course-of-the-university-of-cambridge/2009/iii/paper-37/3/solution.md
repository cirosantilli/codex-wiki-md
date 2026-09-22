<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [classical risk model](../../../../../classical-risk-model.md), let $N(t)$ be the [Poisson process](../../../../../poisson-process.md) of claim arrivals, independent of the independent claim sizes. The reserve starts at $u$ and earns premiums continuously at rate $c$, so

$$
\boxed{U(t)=u+ct-\sum_{i=1}^{N(t)}X_i,\qquad\psi(u)=\mathbb P_u(\tau<\infty),\quad\tau=\inf\{t\ge0:U(t)<0\}.}
$$

Here $\psi$ is the [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) and $\phi=1-\psi$ is the [survival probability](../../../../../survival-probability.md). The [relative safety loading](../../../../../relative-safety-loading.md) is $\theta=(c-\lambda\mu)/(\lambda\mu)>0$.

To derive the [survival integro-differential equation](../../../../../survival-integro-differential-equation-for-a-classical-risk-model.md), condition on the first claim time $T$, which has the [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$. Immediately before that claim the available capital is $u+cT$. A claim $x\le u+cT$ leaves survival probability $\phi(u+cT-x)$, since the future claim process restarts with the same independent law; a larger claim causes ruin immediately. The [first-claim decomposition for survival probability](../../../../../first-claim-decomposition-for-survival-probability.md) is therefore

$$
\phi(u)=\int_0^\infty\lambda e^{-\lambda t}\int_0^{u+ct}\phi(u+ct-x)f(x)\,dx\,dt.
$$

Put $r=\lambda/c$ and $H(v)=\int_0^v\phi(v-x)f(x)dx$. Changing variables to $v=u+ct$ yields

$$
\phi(u)=r e^{ru}\int_u^\infty e^{-rv}H(v)\,dv.
$$

This representation justifies differentiation. The function $H$ is continuous: extend $\phi$ by zero to negative arguments, then use continuity of translations of the integrable density $f$ in $L^1$ to control its convolution with the bounded function $\phi$. Differentiating the lower endpoint of the displayed integral gives $\phi'=r\phi-rH$. Since $c=(1+\theta)\lambda\mu$,

$$
\boxed{\phi'(u)=\frac{\phi(u)}{(1+\theta)\mu}-\frac1{(1+\theta)\mu}\int_0^u\phi(u-x)f(x)\,dx.}
$$

This deduction uses the first-arrival law rather than taking the desired differential equation as an assumption.

For $f(x)=4xe^{-2x}$, the claim law is an [Erlang distribution](../../../../../erlang-distribution.md) of shape two and rate two. Its mean is $\mu=4\int_0^\infty x^2e^{-2x}dx=1$. With $\theta=2$, we have $r=1/3$. Changing the convolution variable to $t=u-x$ gives

$$
H(u)=4e^{-2u}\int_0^u(u-t)\phi(t)e^{2t}dt=4e^{-2u}I(u).
$$

Hence **the first requested specialization** is

$$
\boxed{3\phi'(u)=\phi(u)-4e^{-2u}I(u).}
$$

Let $J(u)=\int_0^u\phi(t)e^{2t}dt$. Differentiation under the finite integral gives $I'=J$ and $J'=\phi e^{2u}$. Differentiating the preceding equation and using $4e^{-2u}I=\phi-3\phi'$ then gives

$$
3\phi''=\phi'+8e^{-2u}I-4e^{-2u}J=-5\phi'+2\phi-4e^{-2u}J.
$$

Thus **the second identity** is

$$
\boxed{3\phi''(u)=-5\phi'(u)+2\phi(u)-4e^{-2u}\int_0^u\phi(t)e^{2t}dt.}
$$

Differentiate once more:

$$
3\phi'''=-5\phi''+2\phi'+8e^{-2u}J-4\phi.
$$

The preceding second-derivative equation gives $8e^{-2u}J=-6\phi''-10\phi'+4\phi$. Substitution cancels the undifferentiated terms and proves

$$
\boxed{3\phi'''+11\phi''+8\phi'=0.}
$$

This is the [Erlang claim-size differential equation for survival probability](../../../../../erlang-claim-size-differential-equation-for-survival-probability.md) with $\beta=2$ and $r=1/3$.

Its characteristic polynomial factors as $z(3z+8)(z+1)$. The limit $\phi(u)\to1$ therefore makes the general bounded solution

$$
\phi(u)=1+A e^{-u}+B e^{-8u/3}.
$$

The supplied [zero-capital survival probability](../../../../../zero-capital-survival-probability.md) is $\phi(0)=2/3$, so $A+B=-1/3$. We also need the initial derivative carried by the original integral equation: $I(0)=0$ implies $\phi'(0)=\phi(0)/3=2/9$, giving $-A-(8/3)B=2/9$. Solving gives $A=-2/5$ and $B=1/15$. Therefore **the survival and ruin probabilities are**

$$
\boxed{\phi(u)=1-\frac25e^{-u}+\frac1{15}e^{-8u/3},\qquad\psi(u)=\frac25e^{-u}-\frac1{15}e^{-8u/3}\quad(u\ge0).}
$$

The extra initial derivative is essential: $\phi(0)$ and the limit at infinity alone would leave one free parameter in the third-order equation. The result has $\psi(0)=1/3$ and tends to zero. It is positive and decreasing, since $\psi'(u)=-(2/5)e^{-u}+(8/45)e^{-8u/3}<0$ for $u\ge0$. These signs agree with its interpretation as an [ultimate ruin probability](../../../../../ultimate-ruin-probability.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
