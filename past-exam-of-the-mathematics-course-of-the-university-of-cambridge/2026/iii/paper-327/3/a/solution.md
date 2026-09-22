<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $P=P_N+P_{N-1}+\cdots+P_0$ as a sum of homogeneous parts. The operator is [elliptic](../../../../../../elliptic-differential-operator.md) when

$$
P_N(\omega)\ne0\qquad\text{for every }\omega\in\mathbb R^n\setminus\{0\}.
$$

Continuity on the [unit sphere](../../../../../../unit-sphere.md) gives $c=\min_{|\omega|=1}|P_N(\omega)|>0$. Uniformly in $\omega$,

$$
t^{-N}P(t\omega)=P_N(\omega)+O(t^{-1}),
$$

so for sufficiently large $t$, $|P(t\omega)|\geq(c/2)t^N$. Since $t^N\asymp\langle t\omega\rangle^N$ at large $t$,

$$
\boxed{|P(\lambda)|\gtrsim\langle\lambda\rangle^N}
$$

for sufficiently large $|\lambda|$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
