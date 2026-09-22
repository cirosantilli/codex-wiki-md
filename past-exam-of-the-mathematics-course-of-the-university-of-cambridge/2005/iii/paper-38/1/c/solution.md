<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The endpoint value printed in this part is erroneous. The correct conclusion is

$$
\boxed{\lim_{t\uparrow1}X_t=0\quad\text{almost surely}}.
$$

Already $\mathbb EX_t^2=t(1-t)\to0$ gives [convergence in probability](../../../../../../convergence-in-probability.md) to zero and rules out an almost sure limit of one.

To prove the stronger endpoint convergence, use [time reversal of a Brownian bridge](../../../../../../time-reversal-of-a-brownian-bridge.md). Set $Y_t=X_{1-t}$, including $Y_0=X_1=0$. Both $X$ and $Y$ are centered [Gaussian processes](../../../../../../gaussian-process.md), and for $s\le t$,

$$
\mathbb E[Y_sY_t]=(1-t)\bigl(1-(1-s)\bigr)=s(1-t).
$$

They therefore have the same finite-dimensional distributions. The path of $X$ is continuous at zero, since its [stochastic integral](../../../../../../stochastic-integral.md) is continuous there. In particular its values at positive rational times tend to zero at zero with probability one. Equality of the laws on the countable rational coordinates transfers this event to $Y$. The path of $Y$ is continuous at every time in $(0,1]$, so its supremum on any interval bounded away from zero is determined by rational times. The rational endpoint condition consequently implies $Y_t\to0$ as $t\downarrow0$ along all real times. Hence $X_t\to0$ as $t\uparrow1$, and setting $X_1=0$ gives a continuous version on the whole closed interval. This proof uses equality of coordinate laws, without assuming terminal continuity in advance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
