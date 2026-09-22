<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a linear, lossless [arterial pressure wave](../../../../../arterial-pressure-wave.md) model with an incompressible fluid of [mass density](../../../../../density.md) $\rho$, small wall [displacement](../../../../../displacement.md) and negligible mean-flow advection compared with the [wave speed](../../../../../wave-speed.md). Let the parent vessel have equilibrium area $A_1$ and speed $c_1$. Linearizing [mass conservation](../../../../../mass-conservation.md) and axial [momentum](../../../../../momentum.md) gives $a_t+A_1u_x=0$ and $\rho u_t=-p_x$. With wall compliance $p=(dp/dA)a$, these imply $c_1^2=(A_1/\rho)dp/dA$. A stiffer wall therefore has larger [wave speed](../../../../../wave-speed.md). A downstream travelling [pressure](../../../../../pressure.md) wave carries flux $Q_+=Y_1p_+$, where $Y_1=A_1/(\rho c_1)$ is the [characteristic admittance of an arterial wave](../../../../../characteristic-admittance-of-an-arterial-wave.md); a returning wave has $Q_-=-Y_1p_-$.

Place the reflecting junction at $x=L$. Treat the daughters as outgoing-wave loads, with combined admittance $Y_d=\sum_jA_j/(\rho c_j)$ and no further returning waves. At the junction, [pressure](../../../../../pressure.md) continuity and flux conservation give $p_I+p_R=p_T$ and $Y_1(p_I-p_R)=Y_dp_T$. Thus the [bifurcation reflection of an arterial pressure wave](../../../../../bifurcation-reflection-of-an-arterial-pressure-wave.md) has

$$
\boxed{r=\frac{p_R}{p_I}=\frac{Y_1-Y_d}{Y_1+Y_d}}.
$$

A decrease in total area gives $0<r<1$ if the parent and daughter [wave speeds](../../../../../wave-speed.md) are equal. More generally this requires $Y_d<Y_1$, an assumption about both area and stiffness. To isolate the effect of ageing, assume all relevant [wave speeds](../../../../../wave-speed.md) increase by the same factor, so their ratios and hence $r$ stay fixed. Unchanged geometry alone does not ensure unchanged $r$ if the vessels stiffen by different factors.

At a station $x<L$, put $\phi=\omega(t-x/c_1)$ and $\vartheta=2\omega(L-x)/c_1$, the round-trip phase to the reflector. The incident [pressure](../../../../../pressure.md) harmonic and its reflection give

$$
p=P_I[\cos\phi+r\cos(\phi-\vartheta)],\qquad Q=Y_1P_I[\cos\phi-r\cos(\phi-\vartheta)].
$$

For time convention $e^{i\phi}$, the two phasors are $P=1+re^{-i\vartheta}$ and $V=1-re^{-i\vartheta}$. Their maximum times are shifted by $-\arg P/\omega$ and $-\arg V/\omega$, respectively. Hence the [pressure-flow phase lag from one arterial reflection](../../../../../pressure-flow-phase-lag-from-one-arterial-reflection.md) is

$$
\boxed{\Delta t=\frac1\omega\operatorname{atan2}(2r\sin\vartheta,1-r^2)}.
$$

Indeed $V/P$ has the argument of $1-r^2+2ir\sin\vartheta$. On the branch $0<\vartheta<\pi$, this phase lag is positive: **the [pressure](../../../../../pressure.md) maximum follows the flow maximum**. There is no cycle-wrap ambiguity on this branch because $1-r^2>0$.

The age trend need not have the same sign at every station. Differentiating the phase gives

$$
\frac{d(\omega\Delta t)}{d\vartheta}=\frac{2r(1-r^2)\cos\vartheta}{(1-r^2)^2+4r^2\sin^2\vartheta}.
$$

Increasing $c_1$ decreases $\vartheta$. At a distal station with $0<\vartheta<\pi/2$, the lag therefore decreases. At a more proximal, ascending-aortic station with $\pi/2<\vartheta<\pi$, it increases. Thus one sufficient set of assumptions reproducing both trends is

$$
\boxed{0<\frac{2\omega(L-x_{\rm distal})}{c_1}<\frac\pi2<\frac{2\omega(L-x_{\rm proximal})}{c_1}<\pi}.
$$

As long as ageing keeps the stations in these ranges, the distal lag falls while the proximal lag rises. The effect is interference between [pressure](../../../../../pressure.md) waves that add and flow waves that subtract, not merely the shortening of one travel time. The lag is largest at a round-trip phase of $\pi/2$.

This is a conditional explanation, with fixed representative harmonic [frequency](../../../../../frequency.md), fixed reflector location, negligible attenuation, negligible additional reflections and common stiffness scaling. The given stiffness and geometry facts alone do not specify the phase ranges, so they do not [force](../../../../../force.md) either age trend without these extra assumptions. Here the two stations lie on the incident-plus-reflected segment. A station beyond the sole junction in an ideal outgoing daughter has only a transmitted wave and zero pressure-flow lag in this model. Actual peripheral measurements beyond that junction require returning waves from further junctions or terminal loads; a single-reflector calculation cannot establish their lag. Non-sinusoidal waveforms, distributed [viscosity](../../../../../dynamic-viscosity.md), mean flow and differently evolving [reflection coefficients](../../../../../reflection-coefficient.md) can also shift peak times. These limitations matter when applying the harmonic explanation to a real arterial network.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
