<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The stochastic quasi-steady-state simulation evolves only $X$:

1. At the current integer $x\geq1$, compute $q(x)=\alpha_3V^2/(\alpha_4x)$ and the averaged rates $\lambda_1(x)=\alpha_1q(x)^2/V$ and $\lambda_2(x)=\alpha_2x(x-1)/V$.  
2. Draw a waiting time $\Delta t\sim\operatorname{Exp}(\lambda_1+\lambda_2)$.  
3. Set $x\leftarrow x+1$ with probability $\lambda_1/(\lambda_1+\lambda_2)$; otherwise set $x\leftarrow x-1$.  
4. Advance time by $\Delta t$ and repeat.

This is a [Gillespie algorithm](../../../../../../gillespie-algorithm.md) for the averaged slow master equation. It samples the fast conditional equilibrium analytically through its factorial moment and never simulates individual fast $Y$ births or deaths.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
