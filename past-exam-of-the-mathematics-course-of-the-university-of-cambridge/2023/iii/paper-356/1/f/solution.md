<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose $\Delta t$ with $\lambda\Delta t\ll1$ and $s\Delta t$ small relative to $L$ and the distance to the target. For each of many independent trajectories:

1. Set $x=y$, $v=s$, and $t=0$.  
2. Propose $x_{\rm new}=x+v\Delta t$.  
3. If $x_{\rm new}\leq0$, record the linearly interpolated target-crossing time and stop. If $x_{\rm new}\geq L$, reflect to $x_{\rm new}=2L-x_{\rm new}$ and set $v=-|v|$.  
4. Otherwise reverse $v$ with probability $1-e^{-\lambda\Delta t}$, set $x=x_{\rm new}$ and $t=t+\Delta t$, and repeat.

The sample mean of the recorded times estimates $\tau^+(y)$. Sampling a Poisson number of reversals and their ordered times inside each step removes the at-most-one-reversal approximation, but the stated Bernoulli scheme converges as $\Delta t\to0$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
