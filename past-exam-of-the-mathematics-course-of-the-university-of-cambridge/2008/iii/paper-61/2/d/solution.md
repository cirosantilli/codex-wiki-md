<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use pulse areas in the convention $\theta_k=\int\Omega_kdt/\hbar$, with the other channel switched off for a single-channel pulse. Substituting $\theta=\pi/2$ into part (c) shows

$$
\boxed{W_1=U_1(\pi/2,\pi/2),\qquad W_2=U_2(\pi/2,-\pi/2).}
$$

Here the arguments denote area and phase. For $W_1$, the off-diagonal factors are $-ie^{-i\pi/2}=-1$ and $-ie^{i\pi/2}=1$. For $W_2$, the phase $-\pi/2$ reverses those two signs. Thus these choices implement the gates exactly on all basis states, not only on one population.

To implement $W_4$, let $P_1=U_1(\pi/2,0)$ and $P_2=U_2(\pi/2,0)$ and apply channel 1, channel 2, then channel 1 again. Each active swap contributes $-i$, so direct tracking gives

$$
P_1P_2P_1|1\rangle=-|3\rangle,\quad
P_1P_2P_1|2\rangle=-|2\rangle,\quad
P_1P_2P_1|3\rangle=-|1\rangle.
$$

Hence $\boxed{W_4=P_1P_2P_1}$, including the overall minus sign and middle-state phase actually printed in the PDF. Alternatively equal zero-phase envelopes give $H(t)=\Omega(t)C$, where $C=E_{12}+E_{21}+E_{23}+E_{32}$. Since $C^3=2C$, its exponential is $I+[(\cos\sqrt2\theta-1)/2]C^2-i(\sin\sqrt2\theta/\sqrt2)C$. One simultaneous pulse with $\theta=\pi/\sqrt2$ gives $I-C^2=-P_{13}=W_4$.

For population transfer alone, the two zero-phase pulses $P_1$ followed by $P_2$ take $|1\rangle\mapsto-i|2\rangle\mapsto-|3\rangle$, so the target population is exactly one. If a positive final amplitude is desired, phases $\phi_1=\phi_2=\pi/2$ give $|1\rangle\mapsto|2\rangle\mapsto|3\rangle$. Both choices require area $\pi/2$ on each channel.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
