<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Treat the [stars](../../../../../star.md) as [point masses](../../../../../point-mass.md) for the orbital motion, neglecting their spin [angular momenta](../../../../../angular-momentum.md). Let $M=M_1+M_2$. Their distances from the [centre of mass](../../../../../center-of-mass.md) are $a_1=aM_2/M$ and $a_2=aM_1/M$. The sum of their orbital [angular momenta](../../../../../angular-momentum.md) is

$$
\begin{aligned}
J&=(M_1a_1^2+M_2a_2^2)\Omega\\
&=\frac{M_1M_2}{M}a^2\left(\frac{GM}{a^3}\right)^{1/2}.
\end{aligned}
$$

Thus the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md) is

$$
\boxed{J=\frac{M_1M_2}{M_1+M_2}\sqrt{G(M_1+M_2)a}.}
$$

For [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), both $M$ and $J$ are fixed. In terms of the [binary mass ratio](../../../../../binary-mass-ratio.md) $q=M_1/M_2$, $M_1=Mq/(1+q)$ and $M_2=M/(1+q)$, hence

$$
J^2=GM^3a\frac{q^2}{(1+q)^4},\qquad\boxed{a(1+q)^{-4}q^2=C,\quad C=\frac{J^2}{GM^3}.}
$$

[Mass conservation](../../../../../mass-conservation.md) also gives $dM_2=-dM_1$, so

$$
\frac{d\log M_2}{d\log M_1}=-q,\qquad\frac{d\log q}{d\log M_1}=1+q.
$$

Differentiating $J\propto M_1M_2a^{1/2}$ at fixed $M,J$ gives $d\log a/d\log M_1=2(q-1)$. Therefore the stipulated [Roche lobe](../../../../../roche-lobe.md) law has the [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md)

$$
\zeta_L=\frac{d\log R_L}{d\log M_1}=\frac3{10}(1+q)+2(q-1)=\frac{23q-17}{10}.
$$

Define the overfill by $\Delta=\log(R_1/R_L)$. On a time scale short compared with the slow change of $K$, the donor's response is $d\log R_1=\beta\,d\log M_1$. Thus

$$
d\Delta=(\beta-\zeta_L)d\log M_1.
$$

During [mass](../../../../../mass.md) loss $d\log M_1<0$. If $\zeta_L>\beta$, [mass](../../../../../mass.md) loss increases the overfill and therefore drives more [mass](../../../../../mass.md) loss: this is positive feedback, giving more rapid [Roche-lobe overflow](../../../../../roche-lobe-overflow.md). If $\zeta_L<\beta$, [mass](../../../../../mass.md) loss decreases the overfill and can balance the slow expansion due to [stellar evolution](../../../../../stellar-evolution.md). More explicitly, with $k_{\mathrm{ev}}=d\log K/dt>0$, contact requires

$$
0=\dot\Delta=k_{\mathrm{ev}}+(\beta-\zeta_L)\frac{\dot M_1}{M_1}.
$$

A slow negative transfer rate can satisfy this only on the stable side $\beta>\zeta_L$. The rapid-transfer condition is therefore

$$
\boxed{q>\frac{17+10\beta}{23}.}
$$

Its time scale depends on the physical donor response represented by $\beta$; it need not be a dynamical time scale if $\beta$ is a thermal-equilibrium mass-radius exponent.

For [Roche-lobe overflow feedback with a constant wind torque factor](../../../../../roche-lobe-overflow-feedback-with-a-constant-wind-torque-factor.md), retain [mass conservation](../../../../../mass-conservation.md) to the stated approximation but allow the prescribed angular-momentum loss. Since $d\log J=f\,d\log M_1$, differentiation gives

$$
f=1-q+\frac12\frac{d\log a}{d\log M_1},\qquad\frac{d\log a}{d\log M_1}=2(q-1+f).
$$

The new [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is

$$
\zeta_L=\frac3{10}(1+q)+2(q-1+f)=\frac{23q-17+20f}{10}.
$$

The same overfill calculation gives

$$
\boxed{q>\frac{17-20f+10\beta}{23}.}
$$

A loss of [angular momentum](../../../../../angular-momentum.md) has $f>0$ because $\dot M_1<0$, and it lowers the critical ratio by making the orbit contract more strongly.

For the specified solar-mass donor exponent $\beta=1/2$, the answer is

$$
\boxed{q>\frac{22-20f}{23},\qquad q>0.}
$$

Without the wind torque this becomes **$q>22/23\simeq0.957$**, so donors slightly less massive than their companions can already lie on the rapid-transfer side of this model. For $0<f<11/10$ the lower threshold is $(22-20f)/23$, and for $f\geq11/10$ every positive $q$ satisfies the strict inequality. There is no finite upper bound on $q$ from this criterion. Since the paper does not specify $f$, the wind case has a conditional range rather than a unique numerical cutoff.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
