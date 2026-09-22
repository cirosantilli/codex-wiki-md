<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The quantities $n_i(\tau,t)$ are [cell-cycle age densities](../../../../cell-cycle-age-density.md): $n_i(\tau,t)\,d\tau$ counts [biological cells](../../../../biological-cell-split.md) whose time since entering phase $i$ lies in $[\tau,\tau+d\tau]$. Here $\tau$ is time spent in the current phase, rather than time since birth. In this two-stage approximation to the [cell cycle](../../../../cell-cycle-split.md), a [biological cell](../../../../biological-cell-split.md) passes from [G1 phase](../../../../g1-phase.md) to [G2 phase](../../../../g2-phase.md), then completes [cell division](../../../../cell-division.md) and produces two daughters entering [G1 phase](../../../../g1-phase.md).

The time [derivative](../../../../derivative.md) measures change at fixed phase age. The age [derivative](../../../../derivative.md) transports [biological cells](../../../../biological-cell-split.md) towards larger $\tau$ at unit speed, because $d\tau/dt=1$. Thus each equation is an [age-structured population equation](../../../../age-structured-population-equation.md). The nonnegative [hazard function](../../../../hazard-function.md) $\Gamma_i(\tau)$ means that, conditional on still being in phase $i$ at age $\tau$, the probability of leaving during the next $dt$ is $\Gamma_i(\tau)dt+o(dt)$. Its product with $n_i$ is the loss from that phase-age class; it is not an additional death term.

The [boundary condition](../../../../boundary-condition.md) at $\tau=0$ specifies the incoming [flux](../../../../flux.md). Every [G1 phase](../../../../g1-phase.md) exit contributes one entrant to [G2 phase](../../../../g2-phase.md), whereas every [G2 phase](../../../../g2-phase.md) exit contributes two entrants to [G1 phase](../../../../g1-phase.md). The [initial conditions](../../../../initial-condition.md) specify the phase-age composition at $t=0$. Consequently [integration](../../../../integral-split.md) over phase age gives the useful population balance

$$
\boxed{\frac{d}{dt}(N_1+N_2)=\int_0^\infty\Gamma_2(\tau)n_2(\tau,t)\,d\tau.}
$$

Each completed [cell division](../../../../cell-division.md) increases the total number of [biological cells](../../../../biological-cell-split.md) by one.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
