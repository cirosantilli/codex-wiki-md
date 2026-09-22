<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The deterministic [SIR model](../../../../../../sir-model.md) follows the [ordinary differential equations](../../../../../../ordinary-differential-equation.md)

$$
\boxed{\dot S=-\beta SI,\qquad\dot I=\beta SI-\gamma I,\qquad\dot R=\gamma I,\qquad(S(0),I(0),R(0))=(N,1,0).}
$$

Use $\beta\ge0$ and $\gamma>0$. The state space is $S,I,R\ge0$, $S+I+R=N+1$; summing the three equations proves conservation of this population. Infection is supported only where $S>0$ and $I>0$, and recovery only where $I>0$. The rates vanish at the corresponding boundaries, preventing negative compartment sizes.

This convention has an unnormalized population infection rate $\beta SI$, as required by the printed threshold. A convention with infection rate $\beta SI/(N+1)$ would use a differently scaled parameter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
