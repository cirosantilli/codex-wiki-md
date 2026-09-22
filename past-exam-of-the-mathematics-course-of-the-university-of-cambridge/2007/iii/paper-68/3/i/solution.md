<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the coupling parameters to be real. The [dipole and quadrupole parity in a mean-field dynamo](../../../../../../dipole-and-quadrupole-parity-in-a-mean-field-dynamo.md) subspaces are invariant: substitution of $A_2=A_1$, $B_2=-B_1$ makes the second-hemisphere equations equal to the first-hemisphere equations with these same signs. Substitution of $A_2=-A_1$, $B_2=B_1$ likewise preserves the other parity. In either subspace put $A=A_1$, $B=B_1$. The reduced equations and characteristic equations are

$$
\begin{aligned}
\text{dipole:}\quad&\dot A=(\alpha_0-\epsilon_1)B-A,\quad
\dot B=(i\Omega-\epsilon_2)A-B,
& (\lambda+1)^2&=(\alpha_0-\epsilon_1)(i\Omega-\epsilon_2),\\
\text{quadrupole:}\quad&\dot A=(\alpha_0+\epsilon_1)B-A,\quad
\dot B=(i\Omega+\epsilon_2)A-B,
& (\lambda+1)^2&=(\alpha_0+\epsilon_1)(i\Omega+\epsilon_2).
\end{aligned}
$$

A marginal [normal mode](../../../../../../normal-mode.md) has $\lambda=i\omega$. Equating real and imaginary parts gives

$$
\begin{aligned}
\text{dipole:}\quad&1-\omega_d^2=-\epsilon_2(\alpha_0-\epsilon_1),
&2\omega_d&=\Omega(\alpha_0-\epsilon_1),\\
\text{quadrupole:}\quad&1-\omega_q^2=\epsilon_2(\alpha_0+\epsilon_1),
&2\omega_q&=\Omega(\alpha_0+\epsilon_1).
\end{aligned}
$$

Consequently the marginal surfaces are

$$
\boxed{F_d=\frac{\Omega^2}{4}(\alpha_0-\epsilon_1)^2-\epsilon_2(\alpha_0-\epsilon_1)=1},\qquad
\boxed{F_q=\frac{\Omega^2}{4}(\alpha_0+\epsilon_1)^2+\epsilon_2(\alpha_0+\epsilon_1)=1}.
$$

To identify which side actually grows, write $z=ab$ in $(\lambda+1)^2=z$. The largest real part of the two [eigenvalues](../../../../../../eigenvalue.md) is $-1+\sqrt{(|z|+\operatorname{Re}z)/2}$. It is negative exactly when $\operatorname{Re}z+[\operatorname{Im}z]^2/4<1$: squaring $|z|<2-\operatorname{Re}z$ proves this, and the latter condition ensures the right-hand side is positive. Thus **dipole modes decay for $F_d<1$ and quadrupole modes decay for $F_q<1$**, with growth for the corresponding reversed inequality.

For explicit [coupled-hemisphere dynamo parity thresholds](../../../../../../coupled-hemisphere-dynamo-parity-threshold.md), suppose $\Omega\ne0$ and define

$$
L=\frac{2\sqrt{\Omega^2+\epsilon_2^2}}{\Omega^2},\qquad
\delta=\epsilon_1+\frac{2\epsilon_2}{\Omega^2}.
$$

The dipole stability interval is $\delta-L<\alpha_0<\delta+L$, and the quadrupole stability interval is $-\delta-L<\alpha_0<-\delta+L$. A comparison of first onset from $\alpha_0=0$ assumes both are initially stable, namely

$$
\boxed{|\delta|<L\quad\Longleftrightarrow\quad
\frac{\Omega^2\epsilon_1^2}{4}+\epsilon_1\epsilon_2<1}.
$$

Increase $|\alpha_0|$ along a specified sign $s=\operatorname{sgn}\alpha_0$. The first thresholds for the two parities are

$$
\boxed{|\alpha_0\Omega|_d=|\Omega|(L+s\delta),\qquad
|\alpha_0\Omega|_q=|\Omega|(L-s\delta)}.
$$

Therefore **the quadrupole reaches onset first if $s(\Omega^2\epsilon_1+2\epsilon_2)>0$; the dipole reaches onset first if it is negative; the thresholds coincide if it vanishes**. For positive $\alpha_0$ and positive coupling parameters this selects the quadrupole, provided the initial stability condition holds. Reversing the sign of $\alpha_0$ exchanges the preference. If both signs are freely allowed, each parity attains the same minimum threshold $|\Omega|(L-|\delta|)$ on opposite sign rays; a unique preference cannot be inferred from the absolute product alone. If the initial stability condition fails, the zero-alpha state is already unstable or marginal and there is no first onset from a stable origin. When $\Omega=0$, the formulas for $F_d,F_q$ still apply, but $|\alpha_0\Omega|$ is identically zero and is not a useful onset parameter.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
