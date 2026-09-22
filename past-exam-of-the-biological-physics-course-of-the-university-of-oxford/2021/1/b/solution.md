<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [two-state ion-channel gating](../../../../two-state-ion-channel-gating.md), write $C\mathrel{\mathop{\rightleftarrows}^{k_o}_{k_c}}O$. Gain minus loss of open [probability](../../../../probability.md) gives the [ordinary differential equation](../../../../ordinary-differential-equation.md)

$$
\dot p_O=k_o(1-p_O)-k_cp_O,\qquad
p_O(t)=p_\infty+[p_O(0)-p_\infty]e^{-t/\tau},\quad
p_\infty=\frac{k_o}{k_o+k_c},\quad \tau=\frac1{k_o+k_c}.
$$

Thus the ratio of the transition rates determines the final open [probability](../../../../probability.md), while their sum determines the response speed. Both given channels have $p_\infty=1/2$. For an initially closed population, with $t$ measured in milliseconds,

$$
\boxed{p_A(t)=\tfrac12(1-e^{-t}),\quad \tau_A=1\,\mathrm{ms};\qquad
p_B(t)=\tfrac12(1-e^{-10t}),\quad \tau_B=0.1\,\mathrm{ms}.}
$$

The mean individual open and closed lifetimes are $1/k_c$ and $1/k_o$: both are $2\,\mathrm{ms}$ for A and $0.2\,\mathrm{ms}$ for B. With the same channel number, single-channel [electrical conductance](../../../../electrical-conductance.md) and driving force, the steady macroscopic [electric currents](../../../../electric-current.md) are equal, but B reaches that value ten times faster. If both populations were already at $p_O=1/2$, neither would show a mean relaxation under these fixed rates: a response also requires an initial condition or a change in rates.

The stationary [variance](../../../../variance-split.md) of the number open is $N/4$ for independent channels. Its [autocovariance](../../../../autocovariance.md) is $(N/4)e^{-|t|/\tau}$, so B's fluctuations decorrelate ten times faster even though their instantaneous [variance](../../../../variance-split.md) is unchanged. Faster gating allows an [ion channel](../../../../ion-channel.md) population to follow a brief stimulus and contribute to rapid [action potential](../../../../action-potential.md) timing. Slower gating integrates over brief changes and can provide a delayed opposing [electric current](../../../../electric-current.md), useful in setting [action potential](../../../../action-potential.md) duration or frequency selectivity. Those examples describe consequences of kinetics; the stipulated voltage-independent rates alone do not define a complete excitable [neuron](../../../../neuron-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
