<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\rho'_{n,j}$ be the $j$th one-system marginal of $\rho'_n$, and put $\varepsilon_n=\|\rho'_n-\rho^{\otimes n}\|_1$. Contractivity of [trace distance](../../../../../../trace-distance.md) under [partial trace](../../../../../../partial-trace.md) gives

$$
\|\rho'_{n,j}-\rho\|_1\leq\varepsilon_n
$$

uniformly in $j$. Because the one-system state space is a [compact space](../../../../../../compact-space.md), continuity of $f(\,\cdot\,\|\sigma)$ implies [uniform continuity](../../../../../../uniform-continuity.md). Hence there is a function $\delta(\varepsilon)\to0$ such that

$$
f(\rho'_{n,j}\|\sigma)
\geq f(\rho\|\sigma)-\delta(\varepsilon_n)
$$

for every $j$.

Multipartite superadditivity and additivity now imply

$$
\begin{aligned}
f(\rho'_n\|\sigma^{\otimes n})
&\geq\sum_{j=1}^nf(\rho'_{n,j}\|\sigma)\\
&\geq n f(\rho\|\sigma)-n\delta(\varepsilon_n),\\
f(\rho^{\otimes n}\|\sigma^{\otimes n})
&=n f(\rho\|\sigma).
\end{aligned}
$$

Therefore

$$
\frac1n\left(
f(\rho'_n\|\sigma^{\otimes n})
-f(\rho^{\otimes n}\|\sigma^{\otimes n})\right)
\geq-\delta(\varepsilon_n)\longrightarrow0,
$$

which proves the required [lower asymptotic semicontinuity of quantum relative entropy](../../../../../../lower-asymptotic-semicontinuity-of-quantum-relative-entropy.md) argument.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
