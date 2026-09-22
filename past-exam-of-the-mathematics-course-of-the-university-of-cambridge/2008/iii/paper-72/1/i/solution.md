<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the gross [star formation rate](../../../../../../star-formation-rate.md) as $\psi=kM_g$, with $k>0$ constant. Use the [instantaneous recycling approximation](../../../../../../instantaneous-recycling-approximation.md): a fraction $F$ returns promptly, while a fraction $1-F$ stays in long-lived [stars](../../../../../../star.md) and remnants. Assume $0\le F<1$, instantaneous mixing, and no [galactic gas inflow](../../../../../../galactic-gas-inflow.md) or [galactic outflow](../../../../../../galactic-outflow.md). If $M_s$ denotes the permanently locked stellar mass, [mass conservation](../../../../../../mass-conservation.md) gives

$$
\dot M_s=(1-F)\psi,\qquad \dot M_g=-(1-F)\psi=-(1-F)kM_g.
$$

Set $\lambda=(1-F)k$. Integration, with $M_g(0)=M_0$, gives the [exponential closed-box gas consumption](../../../../../../exponential-closed-box-gas-consumption.md) law

$$
\boxed{M_g(t)=M_0e^{-\lambda t},\qquad \psi(t)=kM_0e^{-\lambda t}.}
$$

The locked mass is $M_s=M_0(1-e^{-\lambda t})$, so $M_g+M_s=M_0$ at every time. The decay time is $[(1-F)k]^{-1}$, longer than the gross gas-processing time $k^{-1}$ because returned gas can form subsequent generations. The formal $F=1$ limit retains all gas and locks no mass; a finite [stellar yield](../../../../../../stellar-yield.md) defined per locked mass then needs separate treatment.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
