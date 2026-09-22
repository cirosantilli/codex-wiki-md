<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\tau_m=\inf\{s:|X_s|\geq m\}$. The stopped process $X^{\tau_m}$ is bounded, so part (a) gives a continuous adapted quadratic variation $A^{[m]}$. These processes agree before the smaller stopping time, because their dyadic sums agree there and the limits are unique in probability. They therefore paste to a continuous adapted process $A$ with $A_{s\wedge\tau_m}=A_s^{[m]}$.

For fixed $t$ and $\varepsilon>0$,

$$
\mathbb P\left(\sup_{s\leq t}|A_s^{(n)}-A_s|>\varepsilon\right)
\leq\mathbb P(\tau_m\leq t)
+\mathbb P\left(\sup_{s\leq t}|A_s^{(n)}(X^{\tau_m})-A_s^{[m]}|>\varepsilon\right).
$$

The second term tends to zero by part (a), while continuity of $X$ on $[0,t]$ makes $\mathbb P(\tau_m\leq t)\to0$. This proves convergence [uniformly on compact intervals in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
