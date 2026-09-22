<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The odd $X_1$ copy number decreases by two until it reaches one, so $\langle x_1(t)\rangle\to1$. The exact $X_2$ first-moment equation is

$$
\dot m_2
=\alpha_2\langle x_1\rangle
-\alpha_3\langle x_2^2\rangle
-\alpha_7\langle x_2x_4\rangle.
$$

Because copy numbers are [nonnegative integers](../../../../../../natural-number.md), $x_2^2\geq x_2$, and the last mixed moment is nonnegative. Hence

$$
\dot m_2+\alpha_3m_2
\leq\alpha_2\langle x_1\rangle.
$$

The [integrating factor](../../../../../../integrating-factor.md) $e^{\alpha_3t}$, together with $\langle x_1(t)\rangle\to1$, gives the comparison bound

$$
\limsup_{t\to\infty}m_2(t)
\leq\frac{\alpha_2}{\alpha_3}.
$$

Subtracting the exact $X_4$ first-moment equation from the $X_3$ equation cancels reaction 5:

$$
\frac d{dt}\left(\langle x_3\rangle-\langle x_4\rangle\right)
=\alpha_4-\alpha_6m_2(t).
$$

The assumed inequality is precisely

$$
\alpha_4-\alpha_6\frac{\alpha_2}{\alpha_3}>0.
$$

Choose a positive $\varepsilon$ smaller than this gap divided by $\alpha_6$. The [limit superior](../../../../../../limit-superior.md) bound implies that, for all sufficiently large $t$,

$$
\frac d{dt}\left(\langle x_3\rangle-\langle x_4\rangle\right)
\geq
\alpha_4-\alpha_6\left(\frac{\alpha_2}{\alpha_3}+\varepsilon\right)>0.
$$

Thus $\langle x_3\rangle-\langle x_4\rangle$ grows at least linearly. Since $\langle x_4\rangle\geq0$,

$$
\boxed{\lim_{t\to\infty}\langle x_3(t)\rangle=\infty,}
$$

so the required species index is $\boxed{i=3}$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
