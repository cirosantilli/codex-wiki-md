# Finite-gain operational-amplifier integrator

↑ **Parent:** [Op amp integrator](op-amp-integrator.md)

Consider an [op amp integrator](op-amp-integrator.md) with infinite [input impedance](input-impedance.md), an internal controlled voltage $u=-A(s)v$ where $v$ is the inverting-input voltage, and a series [output impedance](output-impedance.md) equal to a resistance $r_o$. Assume no external output load. Writing $y$ for the output, [Kirchhoff's current law](kirchhoff-node-law.md) gives

$$
\frac{v_{\mathrm{in}}-v}{R}=sC(v-y),\qquad \frac{u-y}{r_o}=sC(y-v).
$$

Eliminating $u$ and $v$ yields

$$
\boxed{H(s)=\frac{y}{v_{\mathrm{in}}}=\frac{sCr_o-A(s)}{1+sC\{r_o+R[1+A(s)]\}}.}
$$

The expression at $r_o=0$ is obtained by its limit. In particular, constant gain $A_0$ and $r_o=0$ give $H(s)=-A_0/[1+sRC(1+A_0)]$: a finite direct-current gain followed by an integrating regime. For the dominant-pole model $A(s)=A_0/(1+s/\omega_a)$ and $r_o=0$,

$$
H(s)=\frac{-A_0}{1+s[\omega_a^{-1}+(1+A_0)RC]+s^2RC/\omega_a}.
$$

If $A_0\gg1$ and $A_0\omega_aRC\gg1$, there are separated turnover frequencies near $1/(A_0RC)$ and $A_0\omega_a$. The gain magnitude is respectively constant, proportional to $\omega^{-1}$ and proportional to $\omega^{-2}$. With the convention $e^{i\omega t}$ a continuous phase choice passes from $180^\circ$ through $90^\circ$ to $0^\circ$. If $r_o>0$ and $A(i\omega)\to0$, capacitive feedthrough instead gives the ultimate limit $r_o/(R+r_o)$. Specifying finite gain alone therefore does not specify a unique high-frequency response.

## ↑ Ancestors (8)

1. [Op amp integrator](op-amp-integrator.md)
2. [Operational amplifier](operational-amplifier.md)
3. [Electronic amplifier](electronic-amplifier.md)
4. [Electrical circuit](electrical-circuit-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d12/e/solution.md)
