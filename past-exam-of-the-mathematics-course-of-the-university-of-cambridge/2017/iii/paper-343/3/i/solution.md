<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $n=|\Psi|^2$. Two independent approximations are required for the [reservoir reduction of a polariton condensate](../../../../../../reservoir-reduction-of-a-polariton-condensate.md). First the [exciton](../../../../../../exciton.md) reservoir must follow the changing condensate [number density](../../../../../../number-density.md) rapidly: after its initial transient, its relaxation time $[\gamma_R+R_Rn]^{-1}$ must be small compared with the local density-evolution time. A sufficient modewise condition is that the relevant [number density](../../../../../../number-density.md) frequencies and growth rates are much smaller than $\gamma_R+R_Rn$; pump variations must be comparably slow. There is no reservoir diffusion in the given model. [Adiabatic elimination](../../../../../../adiabatic-elimination.md) then gives

$$
\mathcal R\simeq\frac{P(\mathbf r)}{\gamma_R+R_Rn}.
$$

Second, to obtain the particular cubic equation by expansion about the empty condensate, require $\varepsilon=R_Rn/\gamma_R\ll1$. Then

$$
\mathcal R=\frac P{\gamma_R}\left(1-\frac{R_R}{\gamma_R}n\right)+O\!\left(\frac P{\gamma_R}\varepsilon^2\right).
$$

Keeping the full denominator instead gives a saturable-gain equation, not exactly the requested cubic [complex Ginzburg–Landau equation](../../../../../../complex-ginzburg-landau-equation.md). A near-threshold condensate is one natural regime in which the second condition holds. Rapid reservoir relaxation alone does not justify this [number density](../../../../../../number-density.md) expansion.

Multiplying the condensate equation by $-i$ and inserting the expanded reservoir separates real gain from the conservative frequency shift:

$$
\boxed{\begin{aligned}
\alpha&=\frac12\left(\frac{R_RP}{\gamma_R}-\gamma_C\right),&
\beta&=\frac{R_R^2P}{2\gamma_R^2},\\
g&=U_0-\frac{g_RR_RP}{\gamma_R^2},&
s&=-\frac{g_RP}{\gamma_R}.
\end{aligned}}
$$

These are local functions if the pump is spatially varying. Their signs are important: the reservoir blueshift gives negative $s$ in the printed convention $+is\Psi$, while reservoir depletion subtracts from the effective interaction $g$. Positive rates and pump give $\beta>0$; the effective $g$ need not be positive merely because the original interactions are repulsive.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
