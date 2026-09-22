<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $U=U_0+M-A$ be its [Doob decomposition in discrete time](../../../../../../doob-decomposition-theorem.md) and choose the martingale

$$
X_t^*=-M_t.
$$

Since $Z_t\leq U_t$ and $A_t\geq0$,

$$
Z_t+X_t^*
\leq U_t-M_t
=U_0-A_t
\leq U_0.
$$

For the first optimal stopping time $\tau^*$, the [complementarity for the Snell envelope compensator](../../../../../../complementarity-for-the-snell-envelope-compensator.md) implies $A_{\tau^*}=0$: all compensator increments before $\tau^*$ vanish. Since $Z_{\tau^*}=U_{\tau^*}$,

$$
Z_{\tau^*}+X_{\tau^*}^*=U_0.
$$

Therefore

$$
\max_{0\leq t\leq T}(Z_t+X_t^*)=U_0
$$

pathwise, and taking expectations proves the asserted equality.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
