<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $s=e^{-R\Delta t/L}$ and $J=V/R$, with $0<s<1$. The first interval leaves [electric current](../../../../electric-current.md) $I_1=sI_0$. Position B reconnects the [battery](../../../../electric-battery.md), so the driven [RL circuit](../../../../rl-circuit.md) obeys $L\dot I+RI=V$. Multiplication by the [integrating factor](../../../../integrating-factor.md) $e^{Rt/L}$, or subtraction of the constant solution $J$, gives

$$
I(t)=J+(sI_0-J)e^{-R(t-\Delta t)/L},\qquad \Delta t<t<2\Delta t.
$$

Consequently

$$
\boxed{I_2=s^2I_0+J(1-s).}
$$

The same two intervals give the [recurrence relation](../../../../recurrence-relation.md) $I_{2n+2}=s^2I_{2n}+J(1-s)$. Its [fixed point](../../../../fixed-point.md) is $I_*=J/(1+s)$. Subtracting this [fixed point](../../../../fixed-point.md) makes the [recurrence relation](../../../../recurrence-relation.md) homogeneous:

$$
I_{2n}-I_*=s^{2n}(I_0-I_*),\qquad
\boxed{\lim_{n\to\infty}I_{2n}=\frac{V/R}{1+e^{-R\Delta t/L}}.}
$$

This is the upper endpoint of the eventual [periodically switched RL circuit](../../../../periodically-switched-rl-circuit.md) response, immediately before switching from B to A. The lower endpoint is $sJ/(1+s)$. Their sum is $J$, consistent with equal charging and discharging intervals.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
