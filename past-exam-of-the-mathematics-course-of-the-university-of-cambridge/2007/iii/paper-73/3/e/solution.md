<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the symmetric zero-diagonal weights and asynchronous rule just specified, update only unit $k$. In the energy difference, terms involving neither $k$ nor its symmetric partner cancel. Thus [asynchronous Hopfield energy descent](../../../../../../asynchronous-hopfield-energy-descent.md) gives

$$
\Delta E=-\frac12\sum_{j\ne k}w_{kj}(x_k'-x_k)x_j
-\frac12\sum_{i\ne k}w_{ik}x_i(x_k'-x_k)
=-(x_k'-x_k)h_k.
$$

If the unit was already aligned, it does not change and $\Delta E=0$. If it flips into alignment, $x_k'-x_k=2\operatorname{sgn}(h_k)$, so

$$
\boxed{\Delta E=-2|h_k|<0\quad\text{on every actual non-tie flip}.}
$$

At $h_k=0$ our tie rule retains the old activity. The network has only $2^M$ configurations. Strict descent on every actual change prevents revisiting a configuration and permits only finitely many changes. With a fair schedule every misaligned unit is eventually updated, so the terminal configuration is a fixed point. At that point each possible single-bit flip has energy cost $2x_kh_k\geq0$. **The network reaches a minimum against single-unit changes, not necessarily the global minimum.** Its energy is a [Lyapunov function](../../../../../../lyapunov-function.md) for these asynchronous dynamics.

The qualifications are essential to the printed claim. Synchronous updates can cycle: for two units with $w_{12}=w_{21}=1$, the state $(1,-1)$ alternates with $(-1,1)$, keeping energy $+1$. Symmetry alone therefore does not prove convergence under simultaneous updates.

Nor does the valid descent proof guarantee a global minimum. Consider four units with $w_{12}=w_{34}=3$ and all four cross-group weights equal to $1$, symmetrically and with zero diagonal. The state $(1,1,-1,-1)$ has aligned fields $(1,1,-1,-1)$ and energy $-2$, so it is a strict single-flip local minimum. The all-positive state has energy $-10$. This explicit counterexample shows why local minima may trap retrieval even though the energy always descends under the stipulated rule.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
