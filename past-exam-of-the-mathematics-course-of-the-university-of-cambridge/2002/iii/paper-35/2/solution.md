<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the surplus in the [classical risk model](../../../../../classical-risk-model.md) as $U_t=u+ct-\sum_{j=1}^{N_t}X_j$, with premium rate $c=(1+\rho)\lambda\mu$. The [adjustment coefficient](../../../../../adjustment-coefficient.md) is the positive solution of

$$
\lambda\bigl(M_X(R)-1\bigr)=cR.
$$

For the [exponential distribution](../../../../../exponential-distribution.md) of mean $\mu$, $M_X(r)=(1-\mu r)^{-1}$ for $r<1/\mu$. Cancelling the nonzero root $R$ in its equation gives $\lambda\mu/(1-\mu R)=c$, and hence

$$
\boxed{R=\frac{\rho}{(1+\rho)\mu}.}
$$

It is strictly between zero and $1/\mu$, as required by the transform domain.

The [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) is $\psi(u)=\mathbb P(\inf_{t\ge0}U_t<0)$. The [Lundberg inequality](../../../../../lundberg-inequality.md) states

$$
\boxed{\psi(u)\le e^{-Ru}.}
$$

Ruin can occur only at a claim arrival. Thus the event defining the [finite-claim ruin probability](../../../../../finite-claim-ruin-probability.md) $\psi_n(u)$ is contained in the ultimate ruin event, giving $\psi_n(u)\le\psi(u)\le e^{-Ru}$ for every $n\ge1$ and $u>0$.

For the explicit calculations, take $\mu=1$, put $d=1+\rho=c/\lambda$ and $h=d+1=2+\rho$, and let $T$ be the first arrival time. It has rate-$\lambda$ [exponential distribution](../../../../../exponential-distribution.md), independent of the severity. Ruin on the first claim is the event $X_1>u+cT$, so

$$
\boxed{\psi_1(u)=\mathbb E[e^{-(u+cT)}]=e^{-u}\frac{\lambda}{\lambda+c}=\frac{e^{-u}}h.}
$$

For ruin by the second claim, condition on whether the first claim ruins the insurer or leaves capital $u+cT-x$. The independent future arrivals and severities have the same law as a fresh [classical risk model](../../../../../classical-risk-model.md). Therefore

$$
\begin{aligned}
\psi_2(u)&=\psi_1(u)+\int_0^\infty\lambda e^{-\lambda t}\int_0^{u+ct}e^{-x}\psi_1(u+ct-x)\,dx\,dt\\
&=\frac{e^{-u}}h+\frac{e^{-u}}h\int_0^\infty\lambda e^{-(\lambda+c)t}(u+ct)\,dt\\
&=\boxed{e^{-u}\left(\frac1h+\frac{u}{h^2}+\frac{d}{h^3}\right).}
\end{aligned}
$$

The two terms in the first line refer to disjoint ruin events, so there is no double counting.

For a direct check of the [Lundberg inequality](../../../../../lundberg-inequality.md), now $R=1-1/d$. The ratio $\psi_1(u)/e^{-Ru}=h^{-1}e^{-u/d}$ is less than one. For the second [finite-claim ruin probability](../../../../../finite-claim-ruin-probability.md), put $A=h^{-1}+dh^{-3}$ and $B=h^{-2}$. Its ratio is $e^{-u/d}(A+Bu)$. Since

$$
A-dB=\frac{2d+1}{h^3}>0,\qquad 1-A=\frac{d(h^2-1)}{h^3}>0,
$$

the derivative of this ratio is $e^{-u/d}[B-(A+Bu)/d]<0$ for $u\ge0$, and its value at zero is $A<1$. This verifies both required bounds directly from the calculated probabilities.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
